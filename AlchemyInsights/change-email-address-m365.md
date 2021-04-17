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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819101"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Змінення адреси електронної пошти групи Microsoft 365 або Microsoft Teams

Адресу електронної пошти групи Microsoft 365 або Microsoft Teams можна змінити за допомогою [Центру адміністрування Microsoft 365](https://admin.microsoft.com/). Просто виберіть групу та натисніть @редагувати адресу електронної пошти.

Щоб змінити основну SMTP-адресу групи Microsoft 365 або Teams, можна також скористатися такою командою EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Приклад.

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
