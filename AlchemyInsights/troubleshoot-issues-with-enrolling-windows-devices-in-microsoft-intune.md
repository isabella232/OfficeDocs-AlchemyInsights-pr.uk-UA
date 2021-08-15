---
title: Усунення несправностей із Windows в Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981062"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Усунення несправностей із Windows в Microsoft Intune

Перегляньте наведені нижче ресурси, щоб усунути проблему зараз.
  
Деякі типові повідомлення про помилки та кроки з їх усунення:
  
 **Програмне забезпечення не можна інсталювати, 0x80cf4017:** Термін дії сертифіката вашого облікового запису минув. Повторно завантажте пакет програмного забезпечення "Клієнт ПК" у консолі адміністратора Intune. Докладні відомості див. в цій документації.
  
 **Код помилки 0x801c0003:** Помилка може статися в таких випадках:
  
-  Користувач має більше пристроїв, ніж максимальна кількість пристроїв. Перегляньте ці [документи, щоб видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або змінити обмеження для [пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  Для параметра "Користувачі можуть приєднуватися до пристроїв до Azure AD" установлено значення "немає". Настройте її для всіх або кількох користувачів. Докладні [відомості див. в](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) цій документації.

-  Інший користувач уже затвердив пристрій. У такому разі видаліть пристрій із консолі Azure Intune або вручну спустіть пристрій, перш ніж повторити спробу.

-  Пристрій Windows 10 Home. До Windows 10 Pro, навчальних закладів і підприємств можуть приєднуватися лише Azure Active Directory.

Додаткові ресурси, які допоможуть вирішити вашу проблему:
  
-  На [порталі виправлення неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) можна діагностувати та усунути поширені помилки входу. Перегляньте [цей документ,](https://docs.microsoft.com/intune/help-desk-operators) щоб дізнатися більше.

-  Перегляньте ці документи, де перераховано поширені помилки, які перешкоджають реєстрації, та вирішення для кожної з них: [Посібник із виправлення неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) і [Документ щодо виправлення неполадок](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Дізнайтеся, як Windows пристрої у Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
