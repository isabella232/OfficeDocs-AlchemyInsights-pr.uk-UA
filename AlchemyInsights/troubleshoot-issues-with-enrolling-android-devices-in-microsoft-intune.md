---
title: Виправлення неполадок під час реєстрації пристроїв на платформі Android у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689975"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Виправлення неполадок під час реєстрації пристроїв на платформі Android у Microsoft InTune

Перегляньте наведені нижче ресурси, щоб вирішити проблему.
  
Деякі поширені проблеми та вказівки з вирішення:
  
 **Пристрій не зашифрована помилка на порталі компанії:** Новіші версії Android, зокрема, починаючи з v 7.0, вимагають код запуску, щоб переконатися, що пристрій повністю зашифровано. Загальні рішення дають змогу активувати PIN-код або повністю зашифрувати пристрій. Перегляньте [цей документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , щоб отримати докладні відомості.
  
 **Не вдається виконати вхід за допомогою служби InTune або відображення як "нездорові" в консолі адміністрування inune:** Деякі пристрої Samsung 4,4 і 5,5 можуть не перевіряти в службу. Цю проблему наведено в трьох можливих варіантів:
  
1. Вручну відкрийте програму "портал компанії", яка автоматично ініціюватиме синхронізацію пристрою.

2. Оновіть пристрій до Android 6,0 або новішої версії.

3. Вимкніть програму Samsung Smart Manager від керування порталом компанії Inune. Перегляньте [цей документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , щоб отримати докладні відомості про ці проблеми та способи вирішення.

 Помилка **типу ліцензії користувача** або **ім'я користувача не розпізнано:** користувач має бути призначений ЛІЦЕНЗІЄЮ inune або EMS. Перегляньте ці документи, щоб призначити ліцензію через: Центр адміністрування Office або портал Azure Portal.
  
Додаткові ресурси, які допоможуть вирішити проблему.
  
1. Використовуйте [портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , щоб діагностувати та усунути поширені помилки в реєстрації. Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладні відомості.

2. Перегляньте [цей документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) для списку поширених помилок, які перешкоджають виконанню та дозволах для кожного з них.

3. [Дізнайтеся, як зареєструвати пристрої Android у Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).
