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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679996"
---
# <a name="device-in-pending-state"></a>Пристрій у стані очікування

**Попередні вимоги**

1. Якщо ви вперше налаштували реєстрації пристрою, переконайтеся, що ви переглянули [Загальні відомості про керування пристроями в Лазурому Active Directory (ЛАЗУРНЕ AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , що допоможе вам отримати доступ до пристроїв під елементом керування Azure AD.
2. Якщо ви реєструєте пристрої в Azure AD безпосередньо та вступивши їх у програму Inune, потрібно переконатися, що ви [настроїли](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) програму та маєте [ліцензію](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) на перше місце.
3. Переконайтеся, що ви маєте право виконувати операції в Лазурому та локальному ОГОЛОШЕННІ. Параметри для реєстрації пристроїв можна керувати лише глобальним адміністратором в Лазур AD. Крім того, якщо ви настроїли автоматичну реєстрацію в локальній службі Active Directory, вам потрібно бути адміністратором служби Active Directory та AD FS (якщо це можливо).

Для гібридного процесу реєстрації в процесі об'єднання лазуровий, потрібні пристрої для корпоративної мережі. Вона також працює над VPN, але є деякі застереження. Ми почули клієнтів, які потребують допомоги з усунення несправностей, пов'язаних із процесом реєстрації в гібридному полі Azure, за умовами віддалених робочих умов.

**Середовище автентифікації хмарного середовища (за допомогою синхронізації гешування пароля в Azure AD або передавання автентифікації)**

Цей потік реєстрації також відомий як "Sync JOIN".

Нижче наведено відомості про те, що відбувається під час реєстрації.

1. Операційна система Windows 10 виявляє запис точки з'єднання служби (SCP), коли користувач входить на пристрій.

    1. Спочатку пристрій спробує отримати відомості про клієнта з надбудови "клієнт" у реєстрі [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Докладні відомості наведено в статті [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Якщо це не вдасться, пристрій спілкується з локальною службою Active Directory, щоб отримати відомості про клієнта з SCP. Щоб перевірити, чи передати цей [документ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Ми рекомендуємо ввімкнути SCP у службі Active Directory та лише за допомогою клієнта SCP для початкової перевірки.

2. Операційна система Windows 10 намагається спілкуватися з Azure AD в контексті системи, щоб автентифікувати себе від Azure AD.

    Ви можете перевірити, чи пристрій може отримати доступ до ресурсів Microsoft у системному обліковому записі за допомогою [сценарію підключення випробувального пристрою](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. У Windows 10 створюється Непідписаний сертифікат і зберігається відповідно до об'єкта комп'ютера в локальній службі Active Directory. Для цього потрібно мати можливість прямої видимості для контролера домену.

4. Об'єкт пристрою, який має сертифікат, буде синхронізовано з Azure AD через Azure AD Connect. Цикл синхронізації – кожні 30 хвилин за замовчуванням, але це залежить від конфігурації підключення Azure AD. Щоб отримати докладні відомості, зверніться до цього [документа](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. На цьому етапі ви зможете побачити тему пристрою в розділі "**очікування**" на пристрої з пристрою лазуровий портал.

6. Під час входу в обліковий запис до Windows 10 буде завершено реєстрацію.

    > [!NOTE]
    > Якщо ви працюєте в мережі VPN, а вихід із системи або вхід припиняється, ви можете ініціювати реєстрацію вручну. Для цього виконайте такі дії:
    >
    > Видавати `dsregcmd /join` локально на запит адміністратора або віддалено через Pssexec на свій комп'ютер.
    >
    > Наприклад: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Для поширених проблем із реєстрацією пристроїв Azure Active Directory перегляньте розділ [запитання й відповіді](https://docs.microsoft.com/azure/active-directory/devices/faq).
