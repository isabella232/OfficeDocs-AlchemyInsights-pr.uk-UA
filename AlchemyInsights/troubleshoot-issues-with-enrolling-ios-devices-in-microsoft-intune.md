---
title: Усунення проблем із зарахуванні iOS пристроїв у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736179"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Усунення проблем із зарахуванні iOS пристроїв у Microsoft InTune

Перегляньте ресурси, перелічені нижче, щоб вирішити проблему зараз. 
  
Деякі поширені повідомлення про помилки та дії з роздільною здатністю:
  
- **Досягнуто пристрою Cap** Користувач має більше пристроїв, що надійшли, ніж обмеження пристрою. Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [змінити ліміт пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ця служба не підтримується. Немає реєстрації політика:** Apple Push повідомлення служби (APNS) необхідно налаштувати або поновити. Перегляньте [цей документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , щоб отримати інструкції щодо цього. 
    
- **Неприпустимий тип ліцензії для користувача або ім'я користувача, не розпізнано:** Користувачу потрібно призначити ліцензію InTune або EMS. Перегляньте ці документи, щоб призначити ліцензію через: [Центр адміністрування Office](https://docs.microsoft.com/intune/licenses-assign) або [портал Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Додаткові ресурси, які допоможуть вирішити проблему:
  
1. Для діагностики та вирішення поширених помилок реєстрації скористайтеся [InTune портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) . Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладніші відомості. 
    
2. Перегляньте ці документи, щоб отримати список поширених помилок, які перешкоджають зарахуванням і роздільності до кожного: [посібник із виправлення неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) і [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
3. [Дізнайтеся, як зареєструвати IOS пристроїв у Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).
    

