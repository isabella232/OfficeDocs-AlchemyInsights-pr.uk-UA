---
title: Усунення проблем із зарахуванні пристроїв Windows у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665853"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Усунення проблем із зарахуванні пристроїв Windows у Microsoft InTune

Перегляньте ресурси, перелічені нижче, щоб вирішити проблему зараз.
  
Деякі поширені повідомлення про помилки та дії з роздільною здатністю:
  
 **Не вдається встановити програмне забезпечення, 0x80cf4017:** Термін дії сертифіката облікового запису минув. Повторно завантажити пакет клієнтського програмного забезпечення для комп'ютера, InTune консолі адміністратора. Перегляньте цю документацію, щоб отримати докладнішу інформацію.
  
 **Код помилки 0x801c0003:** Повідомлення про помилку може виникнути в таких випадках:
  
-  Користувач має більше пристроїв, що надійшли, ніж обмеження пристрою. Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [змінити ліміт пристрою](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Користувачі можуть приєднатися до пристроїв Azure AD" встановлено "немає". Встановіть його на всі або виберіть користувачів. Перегляньте [цю документацію](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , щоб отримати докладнішу інформацію.

-  Пристрій уже зареєстровано іншим користувачем. Якщо це так, вийміть пристрій із консолі Azure InTune або вручну скасувати реєстрації пристрою перед повторною спробою.

-  Пристрій Windows 10 Home. Тільки Windows 10 Pro, освіта і підприємство SKUs може приєднатися до Azure Active Directory.

Додаткові ресурси, які допоможуть вирішити проблему:
  
-  Для діагностики та вирішення поширених помилок реєстрації скористайтеся [InTune портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) . Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладніші відомості.

-  Перегляньте ці документи, щоб отримати список поширених помилок, які перешкоджають зарахуванням і роздільності до кожного: [посібник із виправлення неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) і [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Дізнайтеся, як зареєструвати пристрої Windows у програмі Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).
