---
title: Усунення несправностей із записуванням пристроїв Windows у Microsoft Intune
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
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808992"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Усунення несправностей із записуванням пристроїв Windows у Microsoft Intune

Перегляньте наведені нижче ресурси, щоб усунути проблему зараз.
  
Деякі типові повідомлення про помилки та кроки з їх усунення:
  
 **Програмне забезпечення не можна інсталювати, 0x80cf4017:** Термін дії сертифіката вашого облікового запису минув. Повторно завантажте пакет програмного забезпечення "Клієнт ПК" у консолі адміністратора Intune. Докладні відомості див. в цій документації.
  
 **Код помилки 0x801c0003:** Помилка може статися в таких випадках:
  
-  Користувач має більше пристроїв, ніж максимальна кількість пристроїв. Перегляньте ці [документи, щоб видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або змінити обмеження для [пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  Для параметра "Користувачі можуть приєднуватися до пристроїв до Azure AD" установлено значення "немає". Настройте її для всіх або кількох користувачів. Докладні [відомості див. в](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) цій документації.

-  Інший користувач уже затвердив пристрій. У такому разі видаліть пристрій із консолі Azure Intune або вручну спустіть пристрій, перш ніж повторити спробу.

-  Пристрій – це Windows 10 Home. До Azure Active Directory можуть приєднатися лише облікові номери Windows 10 Pro, Education і Enterprise.

Додаткові ресурси, які допоможуть вирішити вашу проблему:
  
-  На [порталі виправлення неполадок Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) можна діагностувати та усунути поширені помилки входу. Перегляньте [цей документ,](https://docs.microsoft.com/intune/help-desk-operators) щоб дізнатися більше.

-  Перегляньте ці документи, щоб отримати список типових помилок, які [](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) запобігають веденю та вирішене проблем із кожним [документом:](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)Посібник із виправлення неполадок і Виправлення неполадок.

[Дізнайтеся, як створити обліковий запис для пристроїв Windows у Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)
