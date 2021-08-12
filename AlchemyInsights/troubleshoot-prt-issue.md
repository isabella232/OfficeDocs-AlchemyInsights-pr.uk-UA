---
title: Усунення несправностей, пов'язаних із PRT
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972737"
---
# <a name="troubleshoot-prt-issue"></a>Усунення несправностей, пов'язаних із PRT

Щоб пройти автентифікацію будь-якого пристрою, він має бути повністю зареєстрований і в хорошому стані, а також мати основний маркер оновлення (PRT).

Щоб реєстрація гібридного об'єднання Azure AD могло бути в корпоративній мережі, пристрої має бути підключено до неї. Він також працює над VPN, але в ньому є певні застереження. Ми почули клієнтів, які потребують допомоги у виправленні несправностей із процесом реєстрації приєднання до гібридної служби Azure AD за обставини віддаленої роботи. Ось розбивка того, що відбувається "під гойданням" в процесі реєстрації.

**Середовище хмарної автентифікації (за допомогою синхронізації гешування паролів Azure AD або натисненої автентифікації)**

Така реєстраційна потік також відома як "Синхронізація приєднатися".

1. Windows 10 виявить запис SCP під час входу користувача на пристрій.
    1. Спочатку пристрій намагається отримати відомості про клієнт із SCP на боці клієнта в реєстрі [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Докладні відомості див. в цьому [документі](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Якщо це не вдасться, пристрій обмінюватися даними з локальною службою Active Directory (AD), щоб отримати відомості про клієнта з точки з'єднання служби (SCP). Щоб підтвердити SCP, перегляньте цей [документ.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Ми радимо вмикати SCP в AD, а для початкової перевірки – лише обліковий запис SCP на боці клієнта.

2. Windows 10 намагається зв'язок з Azure AD в контексті системи, щоб пройти автентифікацію в Azure AD. Ви можете перевірити, чи пристрій може отримати доступ до ресурсів Microsoft із системного облікового запису за допомогою сценарію реєстрації пристроїв.

3. Windows 10 створює самостійно підписаний сертифікат і зберігає його під об'єктом комп'ютера в локальній мережі AD. Для цього потрібно, щоб контролер домену з'являвся на зір.

4. Об'єкт пристрою, який має сертифікат, синхронізується з Azure AD через Azure AD Підключення. Цикл синхронізації за замовчуванням триває кожні 30 хвилин, але це залежить від конфігурації Azure AD Підключення. Докладні відомості див. в цьому [документі.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. На цьому етапі тематичний пристрій має з'явитись у стані "Очікує" у розділі blade of Device blade of Azure Portal (Очікується).

6. Під час наступного входу Windows 10 буде завершено реєстрацію. 

> [!NOTE]
> Якщо ви ввійшли до мережі VPN, а процес входу з логотипом припиняє підключення до домену, ви можете ініціювати реєстрацію вручну:
 1. Видачі dsregcmd /join локально за допомогою запиту адміністратора або віддалено за допомогою PSExec на ПК. Наприклад, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Докладні відомості про проблеми з гібридним приєднанням див. в [розділах Усунення несправностей пристроїв.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
