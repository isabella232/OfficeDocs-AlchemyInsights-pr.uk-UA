---
title: Змінення адреси електронної пошти групи Microsoft 365
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819065"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Змінення адреси електронної пошти групи Microsoft 365

Адресу електронної пошти групи Microsoft 365 можна змінити в Центрі адміністрування. Просто виберіть групу та натисніть @редагувати адресу електронної пошти.

Щоб змінити основну SMTP-адресу групи Microsoft 365, можна також скористатися командою EXO PowerShell:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Приклад.

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
