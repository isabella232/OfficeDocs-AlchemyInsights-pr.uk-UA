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
ms.openlocfilehash: 0a07e6279f533a4c26a4e90c10651421a5df8860
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/27/2020
ms.locfileid: "44283265"
---
# <a name="change-email-address-of-an-microsoft-365-group"></a>Змінення адреси електронної пошти групи Microsoft 365

Можна змінити адресу електронної пошти групи Microsoft 365 за допомогою Центру адміністрування. Просто виберіть групу і виберіть @edit адресу електронної пошти.

Ви також можете використовувати наступні команди EXO PowerShell для зміни основна адреса SMTP групи Microsoft 365:

Набір-UnifiedGroup <Group Name> -первинний, адресадреса<new SMTP Address>

Приклад:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
