---
title: Я блокую умовний доступ із пристроєм, який несумісний
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019169"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>Я блокую умовний доступ із пристроєм, який несумісний

**Рекомендовані інструменти з високим пріоритетом**

- [Засіб усунення неполадок реєстрації пристроїв](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – вичерпний засіб, який допомагає вирішити найпоширеніші проблеми з реєстрацією пристроїв.
- [Сценарій реєстрації пристроїв .](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) Засіб, який використовується для забезпечення доступу до кінцевих точок реєстрації пристроїв у системному обліковому записі.
- [Сценарій очищення пристрою Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – засіб, який використовується для пошуку застарілих пристроїв у середовищі та керування ними.

Нижче наведено деякі поширені причини того, чому умовний доступ може не вдатися на пристрої, що працює на основі вимоги, або чому користувачі можуть отримувати повідомлення Звідси не можна отримати доступ під час запиту на вхід до ресурсу організації. 

1. **Пристрій не має обов'язкового стану пристрою з MDM:**

Підтвердьте, що пристрій зараховано до затвердженого постачальника MDM, наприклад Intune, і позначте його як *відповідний.* Докладні відомості про Intune див. в цьому [документі.](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) Докладні відомості про відповідність пристроїв і Intune див. в розділі Налаштування правил для пристроїв, для керування ними за допомогою Intune за допомогою [політики відповідності.](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started) Якщо у вас виникають проблеми під час деталізації пристрою з Intune, знайдіть відомості про виправлення неполадок у статті Усунення несправностей із записуванням пристрою [в Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Для подальшої підтримки Intune створіть запит на підтримку. Для цього перейдіть на сторінку довідки та підтримки [Intune.](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)

2. **Пристрій не приєднано до мережі організацій:**

Щоб отримати доступ до ресурсів організації, пристрій має бути підключено до мережі організації через пряме підключення або віртуальну приватну мережу (VPN), а також підключений до локальної або Azure Active Directory. Щоб дізнатися, як приєднати робочий пристрій до мережі організації, див. номери Приєднання робочого [пристрою до мережі організації.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) Відомості про реєстрацію особистого або byOD-пристрою див. в статтях Реєстрація особистого пристрою [в мережі організації.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)

- Щоб перевірити, чи пристрій приєднався до мережі, можна виконати вказівки для зареєстрованих пристроїв тут або [на](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) робочих [пристроях тут.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) Щоб знизити кількість проблем із підключенням до мережі в мережі Org, дотримуйтеся наведених нижче рекомендацій.

    1. Увійдіть у Windows за допомогою робочого або навчального облікового запису, наприклад alain@contoso.com.
    2. Підключення мережі організації через мережу VPN або DirectAccess.
    3. Після підключення натисніть клавіші **Windows+L,** щоб заблокувати пристрій.
    4. Розблокуйте пристрій за допомогою робочого або навчального облікового запису, а потім знову спробуйте отримати доступ до проблемної програми або служби.

Якщо **з'явиться** повідомлення про помилку Не вдається отримати тут знову, імовірно, проблема в іншому місці.

3. **Операційна система не підтримується:**

Переконайтеся, що ви використовуєте підтримувану версію операційної системи, зокрема:

- **Windows клієнта:** Windows 7 або пізнішої версії

- **Windows Server**: Windows Server 2008 R2 або пізніша версія

- **macOS**: macOS X або пізнішої версії

- **Android та iOS:** найновіша версія мобільних операційних систем Android і iOS

4. **Браузер не підтримується:**

Нижче наведено підтримувані браузери. Для підтримки Chrome в Windows версії 1703 або новішої версії Windows 10 потрібно вказувати розширення Облікові записи. Для Edge 85 і більше користувач має ввійти, щоб належним чином пройти перевірку відповідності пристрою. Докладні відомості див. [тут.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

- **Windows 10:** Microsoft Edge, Internet Explorer, Chrome
- **Windows 8 / 8.1:** Internet Explorer, Chrome
- **Windows 7:** Internet Explorer, Chrome
- **iOS**: Microsoft Edge, Intune Managed Browser, Safari
- **Android**: **Microsoft Edge**: Керований браузер Intune, Chrome
- **Windows Phone:** Microsoft Edge, Internet Explorer
- **Windows Server 2019:** Microsoft Edge, Internet Explorer, Chrome
- **Windows Server 2016:** Internet Explorer
- **Windows Server 2012 R2:** Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome, Safari

Докладні відомості про те, як це **зробити,** див. [тут.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)
