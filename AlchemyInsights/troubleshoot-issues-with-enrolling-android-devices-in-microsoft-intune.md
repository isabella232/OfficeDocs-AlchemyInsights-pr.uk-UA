---
title: Усунення несправностей із записуванням пристроїв Android у Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830963"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Усунення несправностей із записуванням пристроїв Android у Microsoft Intune

Перегляньте наведені нижче ресурси, щоб усунути проблему зараз.
  
Нижче наведено деякі поширені проблеми та спосіб вирішення.
  
 **Помилка пристрою, не зашифрованого на порталі компанії:** Щоб повністю шифрувати пристрій, у новіших версіях Android, особливо починаючи з версії 7.0, потрібен код допуску. Поширені рішення дають змогу ввімкнути pin-код запуску або повністю шифрувати пристрій. Перегляньте [цей документ,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) щоб отримати докладніші відомості.
  
 Не вдається перевірити пристрій за допомогою служби Intune або відобразити стан "Несприятливий" у консолі **адміністратора Intune:** Деякі пристрої Samsung 4.4 та 5.5 можуть не потрапити до служби. Цю проблему можна вирішити 3 способами:
  
1. Вручну відкрийте програму Intune Company Portal, яка автоматично ініціюватиме синхронізацію пристроїв.

2. Оновіть пристрій до Android 6.0 або новішої версії.

3. Вимкніть Samsung Smart Manager на порталі компанії Intune. Перегляньте [цей документ,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) щоб отримати додаткові відомості про ці проблеми та вирішення.

 **Помилка "Тип ліцензії користувача"** Неприпустимий або Не розпізнано ім'я **користувача:** користувачу потрібно призначити ліцензію Intune або EMS. Перегляньте ці документи, щоб призначити ліцензію через: Центр адміністрування Office або портал Azure.
  
Додаткові ресурси, які допоможуть вирішити вашу проблему:
  
1. На [порталі виправлення неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) можна діагностувати та усунути поширені помилки входу. Перегляньте [цей документ,](https://docs.microsoft.com/intune/help-desk-operators) щоб дізнатися більше.

2. Перегляньте [цей документ,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) щоб переглянути список типових помилок, які запобігають їй в списках і їх вирішення.

3. [Дізнайтеся, як затвердити пристрої Android у Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
