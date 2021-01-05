---
title: Змінення адреси електронної пошти групи Microsoft 365 або Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756578"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Змінення адреси електронної пошти групи Microsoft 365 або Microsoft Teams

Адресу електронної пошти групи Microsoft 365 або Microsoft Teams можна змінити за допомогою [Центру адміністрування Microsoft 365](https://admin.microsoft.com/). Просто виберіть групу та натисніть @редагувати адресу електронної пошти.

Щоб змінити основну SMTP-адресу групи Microsoft 365 або Teams, можна також скористатися такою командою EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Приклад.

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
