---
title: Усунення проблем із зарахуванні пристроїв Android у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759641"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Усунення проблем із зарахуванні пристроїв Android у Microsoft InTune

Перегляньте ресурси, перелічені нижче, щоб вирішити проблему зараз.
  
Деякі поширені проблеми та вирішення кроки:
  
 **Пристрій не зашифрована помилка в порталі компанії:** Новіші версії Android, зокрема починаючи з версії 7.0, вимагають завантаження пароля, щоб переконатися, що пристрій повністю зашифровано. Загальними рішеннями є ввімкнення PIN-коду або повного шифрування пристрою. Перегляньте [цей документ](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , щоб отримати додаткові відомості.
  
 **Пристрої не вдається перевірити за допомогою служби InTune або відображення як "нездоровий" у консолі адміністратора InTune:** Деякі пристрої Samsung 4,4 та 5,5 можуть не перевіряти в сервісі. Є 3 варіанти вирішення цієї проблеми:
  
1. Вручну відкрийте програму портал компанії InTune, яка автоматично ініціюватиме синхронізацію пристрою.

2. Оновіть пристрій до Android 6,0 або новішої.

3. Вимкніть Samsung Smart Manager, з керування портал компанії InTune. Перегляньте [цей документ](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , щоб отримати додаткові відомості про ці проблеми та рішення.

 **Неприпустимий тип ліцензії** або **ім'я користувача не розпізнано помилка:** користувачу необхідно ПРИЗНАЧИТИ ліцензію InTune або EMS. Перегляньте ці документи, щоб призначити ліцензію через: Центр адміністрування Office або портал Azure.
  
Додаткові ресурси, які допоможуть вирішити проблему:
  
1. Для діагностики та вирішення поширених помилок реєстрації скористайтеся [InTune портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) . Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладніші відомості.

2. Перегляньте [цей документ](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) для списку поширених помилок, які перешкоджають реєстрації та роздільності.

3. [Дізнайтеся, як зареєструвати Android пристроїв у Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).
