---
title: Приховання або приховання Office 365 груп або команд зі списку адрес
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088417"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Приховання або приховання Office 365 груп або команд зі списку адрес

Щоб приховати або відобразити групи Office 365 або команди в списках адрес (GAL) клієнтів Exchange (Outlook, OWA), використовуйте таку команду EXO PowerShell:

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Щоб приховати або приховати групи Або команди Office365 у клієнтських програмах Exchange (Outlook, OWA), використовуйте таку команду EXO PowerShell:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Докладні вказівки див. [в статті Приховання Office 365 груп у списку GAL і Exchange клієнтів.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
