---
title: Змінення адреси електронної пошти групи Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580678"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Змінення адреси електронної пошти групи Microsoft 365

Можна змінити адресу електронної пошти групи Microsoft 365 за допомогою Центру адміністрування. Просто виберіть групу і виберіть @edit адресу електронної пошти.

Ви також можете використовувати наступні команди EXO PowerShell для зміни основна адреса SMTP групи Microsoft 365:

Набір-UnifiedGroup <Group Name> -первинний, адресадреса<new SMTP Address>

Приклад:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
