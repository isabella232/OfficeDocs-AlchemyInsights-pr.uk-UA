---
title: Змінення адреси електронної пошти групи Microsoft 365 або Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995643"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Змінення адреси електронної пошти групи Microsoft 365 або Microsoft Teams

Адресу електронної пошти групи Microsoft 365 або Microsoft Teams можна змінити за допомогою [Центру адміністрування Microsoft 365](https://admin.microsoft.com/). Просто виберіть групу та натисніть @редагувати адресу електронної пошти.

Щоб змінити основну SMTP-адресу групи Microsoft 365 або Teams, можна також скористатися такою командою EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Приклад.

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
