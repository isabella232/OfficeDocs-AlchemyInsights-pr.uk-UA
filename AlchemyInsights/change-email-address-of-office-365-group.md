---
title: Змінення адреси електронної пошти групи Microsoft 365 пошти
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
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930750"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Змінення адреси електронної пошти групи Microsoft 365 пошти

Адресу електронної пошти групи Microsoft 365 можна змінити в Центрі адміністрування. Просто виберіть групу та натисніть @редагувати адресу електронної пошти.

Щоб змінити основну SMTP-адресу групи, можна також скористатися Microsoft 365 EXO PowerShell:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Приклад.

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
