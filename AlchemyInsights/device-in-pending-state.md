---
title: Пристрій у стані очікування
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330393"
---
# <a name="device-in-pending-state"></a>Пристрій у стані очікування

**Передумови:**

1. Якщо ви налаштували реєстрацію пристроїв уперше, переконайтеся, що ви переглянули загальні відомості про керування пристроями в [Azure Active Directory (Azure AD),](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) де ви зможете отримати пристрої під контролем Azure AD.
2. Якщо ви реєструєте пристрої безпосередньо в Azure AD та зареєстрували їх в Intune, переконайтеся, [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) що ви налаштували [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) і ліцензування настроїли спочатку.
3. Переконайтеся, що ви маєте право виконувати операції в Azure AD та локальному середовищі AD. Тільки глобальний адміністратор Microsoft Azure AD може керувати параметрами реєстрації пристроїв. Крім того, щоб налаштувати автоматичну реєстрацію в локальній службі Active Directory, вам потрібно мати права адміністратора служби Active Directory та AD FS (якщо застосовується).

Щоб реєстрація гібридного об'єднання Azure AD могло бути в корпоративній мережі, пристрої має бути підключено до неї. Він також працює над VPN, але в ньому є певні застереження. Ми почули, що клієнтам потрібна допомога з виправлення неполадок реєстрації гібридного об'єднання Azure AD за віддалених обставин роботи.

**Середовище хмарної автентифікації (за допомогою синхронізації гешування паролів Azure AD або натисненої автентифікації)**

Така реєстраційна потік також відома як "Синхронізація приєднатися".

Нижче наведено ієрархічну процедуру реєстрації.

1. Windows 10 виявляє запис SCP-сервера під час входу користувача на пристрій.

    1. Пристрій спочатку намагається отримати відомості про клієнт із SCP на боці клієнта в реєстрі [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Докладні відомості див. в [документі](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Якщо це не вдасться, пристрій зв'язуватимуться з локальною службою Active Directory, щоб отримати відомості про клієнта від SCP. Щоб підтвердити SCP, ознайомтесь із цим [документом.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    **Примітка.** Для початкової перевірки радимо вмикати SCP в Active Directory, використовуючи лише обліковий запис SCP на боці клієнта.

2. Windows 10 намагається зв'язок з Azure AD в контексті системи, щоб пройти автентифікацію в Azure AD.

    Ви можете перевірити, чи пристрій може отримати доступ до ресурсів Microsoft із системного облікового запису за допомогою [сценарію реєстрації пристроїв.](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)

3. Windows 10 створює самостійно підписаний сертифікат і зберігає його під об'єктом комп'ютера в локальній службі Active Directory. Для цього потрібно, щоб контролер домену з'являвся на зір.

4. Об'єкт пристрою, який має сертифікат, синхронізується з Azure AD через Azure AD Підключення. Цикл синхронізації за замовчуванням триває кожні 30 хвилин, але це залежить від конфігурації Azure AD Підключення. Докладні відомості див. в цьому [документі.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. На цьому етапі пристрій має з'явитись у стані **"Очікує"** в розділі blade of Azure Portal (Очікується).

6. Під час наступного входу Windows 10 буде завершено реєстрацію.

    **Примітка.** Якщо ви ввійшли у VPN і емблема або вхід припиняє підключення до домену, ви можете ініціювати реєстрацію вручну. Ось як це зробити:
    
    Видачі локально за допомогою запиту адміністратора або віддалено за допомогою `dsregcmd /join` PSExec на ПК.\
    Наприклад: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Поширені проблеми з реєстрацією Azure Active Directory пристроїв див. в [статті Пристрої: запитання й відповіді.](https://docs.microsoft.com/azure/active-directory/devices/faq)
