---
title: Усунення несправностей, пов'язаних із Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047997"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Усунення несправностей, пов'язаних із Microsoft Intune

Перегляньте наведені нижче ресурси, щоб усунути проблему зараз. 
  
Деякі типові повідомлення про помилки та кроки з їх усунення:
  
- **Досягнуто максимальної потужності пристрою** Користувач має більше пристроїв, ніж максимальна кількість пристроїв. Перегляньте ці [документи, щоб видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або змінити обмеження для [пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ця служба не підтримується. Немає політики членство.** Потрібно налаштувати або поновити службу push-сповіщень Apple. Перегляньте [цей документ,](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) щоб дізнатися, як це зробити. 
    
- **Неприпустимий тип ліцензії користувача або не розпізнано ім'я користувача:** Користувачу потрібно призначити ліцензію Intune або EMS. Перегляньте ці документи, щоб призначити ліцензію через: [Office порталі](https://docs.microsoft.com/intune/licenses-assign) [Адміністрування або Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Додаткові ресурси, які допоможуть вирішити вашу проблему:
  
1. На [порталі виправлення неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) можна діагностувати та усунути поширені помилки входу. Перегляньте [цей документ,](https://docs.microsoft.com/intune/help-desk-operators) щоб дізнатися більше. 
    
2. Перегляньте ці документи, де перераховано поширені помилки, які перешкоджають реєстрації, та вирішення для кожної з них: [Посібник із виправлення неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) і [Документ щодо виправлення неполадок](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Дізнайтеся, як затвердити пристрої з iOS у Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)
    

