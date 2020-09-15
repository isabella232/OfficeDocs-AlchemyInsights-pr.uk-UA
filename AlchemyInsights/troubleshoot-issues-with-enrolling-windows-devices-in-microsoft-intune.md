---
title: Виправлення неполадок під час реєстрації пристроїв Windows у Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658899"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Виправлення неполадок під час реєстрації пристроїв Windows у Microsoft InTune

Перегляньте наведені нижче ресурси, щоб вирішити проблему.
  
Деякі поширені повідомлення про помилки та роздільну здатність:
  
 **Не вдалося інсталювати програмне забезпечення, 0x80cf4017:** Термін дії сертифіката облікового запису завершився. Повторно завантажте пакет програмного забезпечення для клієнта ПК в консолі адміністратора Inune. Перегляньте цю документацію, щоб отримати докладніші відомості.
  
 **Код помилки 0x801c 0003:** Помилка може виникати в таких ситуаціях:
  
-  Користувач має більше пристроїв, зарахованих, ніж обмеження на пристрій. Перегляньте ці документи, щоб [Видалити пристрій](https://docs.microsoft.com/intune/devices-wipe) або [Змінити обмеження на пристрій](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Користувачі можуть приєднатися до пристрою в Azure AD" "ні". Установіть або виберіть елемент користувачі. Перегляньте [цю документацію](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , щоб отримати докладніші відомості.

-  Пристрій уже зареєстровано іншим користувачем. Якщо це так, видаліть пристрій із консолі Azure Inune або вручну скасуйте реєстрацію пристрою, перш ніж намагатися ще раз.

-  Пристрій – це Windows 10 Home. Приєднатися до "Azure Active Directory" можна лише в ОС Windows 10 Pro, освіті та підприємстві SKUs.

Додаткові ресурси, які допоможуть вирішити проблему.
  
-  Використовуйте [портал виправлення неполадок](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , щоб діагностувати та усунути поширені помилки в реєстрації. Перегляньте [цей документ](https://docs.microsoft.com/intune/help-desk-operators) , щоб отримати докладні відомості.

-  Перегляньте ці документи для списку поширених помилок, які перешкоджають виконанню та резолюціям кожного з них: [посібник із виправлення неполадок](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) і [Виправлення неполадок із документами](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Дізнайтеся, як зареєструвати пристрої Windows у Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).
