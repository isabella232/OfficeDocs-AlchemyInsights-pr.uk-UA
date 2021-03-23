---
title: У мене заблоковано умовний доступ із сумісним пристроєм
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
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037081"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>У мене заблоковано умовний доступ із сумісним пристроєм

**Високорекомендовані інструменти**

- Засіб [вирішення проблем із реєстрацією пристроїв](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – це вичерпний засіб, який допомагає усувати найпоширеніші проблеми з реєстрацією пристроїв.
- [Скрипт підключення пристрою для тестування](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – це засіб, який використовується для того, щоб пристрій міг отримати доступ до кінцевих точок реєстрації пристрою в системному обліковому записі.
- [Сценарій очищення пристрою Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) – це засіб, який використовується для пошуку та керування застарілою пристроями в навколишньому середовищі.

Нижче наведено кілька типових причин, через які умовний доступ може не працювати з сумісним пристроєм, а також про те, чому ваші користувачі можуть отримувати **доступ** до цього повідомлення під час запиту на вхід до організаційного ресурсу.

1. **Пристрій не має необхідного стану пристрою з використанням MDM**:

Перевірте, чи пристрій зареєстровано в затвердженому постачальника MDM, наприклад Inune, і *позначений як сумісний*. Щоб отримати докладніші відомості про Inune, перегляньте цей [документ](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment). Щоб краще зрозуміти відповідність пристрою та виконати наведені нижче відомості, ознайомтеся [з політикою відповідності, щоб указати правила для пристроїв, за допомогою яких можна керувати з Inune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started). Якщо виникають проблеми під час реєстрації пристрою з Inune, Дізнайтеся про виправлення неполадок під [час реєстрації пристрою в корпорації Майкрософт](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune). Для подальшої підтримки Inune створіть запит на підтримку. Щоб зробити це, перейдіть на [сторінку довідки та підтримки на сторінці Inune](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).

2. **Пристрій не приєднується до мережі організацій**:

Щоб отримати доступ до організаційних ресурсів, пристрій має бути підключений до мережі організації, за допомогою прямого підключення або віртуальної приватної мережі (VPN), а також до локального або блакитного Active Directory. Щоб приєднатися до мережі з робочим пристроєм, зверніться до [свого робочого пристрою в мережу організації](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network). Щоб зареєструвати пристрій особистого/BYOD, див. [Реєстрація особистого пристрою в мережі організації](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).

- Щоб перевірити, чи підключений пристрій до мережі, виконайте вказівки для зареєстрованих пристроїв [тут](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) або робочих пристроїв [тут](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined). Щоб зробити цю проблему в організаційній мережі, виконайте наведені нижче вказівки.

    1. Увійдіть у Windows за допомогою робочого або навчального облікового запису, наприклад alain@contoso.com.
    2. Підключення до мережі організації через VPN або DirectAccess.
    3. Після підключення натисніть клавішу з **емблемою Windows + L** , щоб заблокувати пристрій.
    4. Розблокуйте свій пристрій за допомогою робочого або навчального облікового запису, а потім спробуйте отримати доступ до проблемної програми або служби ще раз.

Якщо відображається повідомлення про помилку, можливо, проблему ще **не вдається отримати** , проблема може бути в іншому місці.

3. **Операційна система не підтримується**:

Переконайтеся, що ви використовуєте підтримувану версію операційної системи, зокрема:

- **Клієнт Windows**: операційна система Windows 7 або пізніша

- **Windows Server**: windows Server 2008 R2 або пізніша версія

- **MacOS**: MacOS X або пізніша версія

- **Android і IOS**: Найновіша версія операційної системи Android і IOS для мобільних пристроїв

4. **Веб-браузер не підтримується**:

Нижче наведено наведені нижче браузери, які підтримуються нижче. Для підтримки Chrome у Windows 1703 або пізніші версії необхідно мати розширення облікових записів Windows 10. Для EDGE 85 + потрібно ввійти в систему, щоб належним чином передавати відомості про відповідність пристрою. Щоб отримати докладніші відомості, ознайомтеся з наведеними [тут](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).

- **Windows 10**: Microsoft EDGE, Internet Explorer, Chrome
- **Windows 8/8,1**: Internet Explorer, Chrome
- **Windows 7**: Internet Explorer, Chrome
- **IOS**: Microsoft EDGE, Inune керований браузер, Safari
- **Android**: **Microsoft EDGE**: Inune кероване браузера, хром
- **Windows Phone**: Microsoft EDGE, Internet Explorer
- **Windows Server 2019**: Microsoft EDGE, Internet Explorer, Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: хром, Safari

Дізнайтеся більше про те, що **ви не можете отримати доступ** до повідомлень [і інструкцій з](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)виправлення неполадок.
