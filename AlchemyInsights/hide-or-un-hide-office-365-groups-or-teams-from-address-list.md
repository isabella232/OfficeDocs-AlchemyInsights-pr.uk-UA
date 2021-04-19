---
title: Приховання або приховання груп і команд Office 365 у списку адрес
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811477"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Приховання або приховання груп і команд Office 365 у списку адрес

Щоб приховати або приховати групи Office 365 або команди в списках адрес (GAL) клієнтів Exchange (Outlook, OWA), використовуйте наведену нижче команду EXO PowerShell.

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Щоб приховати або приховати групи Office365 або команди в клієнтах Exchange (Outlook, OWA), використовуйте таку команду EXO PowerShell:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Докладні вказівки див. [в статті Приховання груп Office 365 у клієнтах GAL і Exchange.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
