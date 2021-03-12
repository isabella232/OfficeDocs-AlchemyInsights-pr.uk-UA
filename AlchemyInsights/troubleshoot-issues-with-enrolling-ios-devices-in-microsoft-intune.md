---
title: Виправлення неполадок під час реєстрації пристроїв з iOS у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708983"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Виправлення неполадок під час реєстрації пристроїв з iOS у Microsoft InTune

Перегляньте наведені нижче ресурси, щоб вирішити проблему. 
  
Деякі поширені повідомлення про помилки та роздільну здатність:
  
- Пристрій, на якому **досягнуто кришку** Користувач має більше пристроїв, зарахованих, ніж обмеження на пристрій. Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [Змінити обмеження на пристрій](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ця служба не підтримується. Немає політики реєстрації:** ви повинні настроїти або поновити службу сповіщень Apple Push (APNS). Перегляньте [цей документ](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , щоб отримати вказівки щодо того, як це зробити. 
    
- **Неприпустимий тип ліцензії користувача або ім'я користувача не розпізнано:** Користувачу потрібно призначити ліцензію "Inune" або "EMS". Перегляньте ці документи, щоб призначити ліцензію через: [Центр адміністрування Office](https://docs.microsoft.com/intune/licenses-assign) або [портал Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Додаткові ресурси, які допоможуть вирішити проблему.
  
1. Використовуйте [портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , щоб діагностувати та усунути поширені помилки в реєстрації. Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладні відомості. 
    
2. Перегляньте ці документи для списку поширених помилок, які перешкоджають виконанню та резолюціям кожного з них: [посібник із виправлення неполадок](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) і [Виправлення неполадок із документами](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Дізнайтеся, як зареєструвати пристрої з iOS у Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).
    

