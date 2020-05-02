---
title: Приватний канал
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005459"
---
# <a name="private-channels-in-microsoft-teams"></a>Приватні канали у Microsoft teams

Приватні канали – це нова функція у Microsoft teams. Зауважте, що приватні канали не можна конвертувати зі стандартних каналів або навпаки.

Щоб отримати докладні відомості про приватні канали, такі як інформація про [створення приватних каналів і членство](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) та [приватний канал SharePoint сайтів](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), перегляньте [приватні канали в Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Примітка:** Оскільки конфігурація для збереження повідомлень приватного каналу ще не підтримується, орендарі з увімкнутими політиками збереження не матимуть приватних каналів, увімкнуті за замовчуванням. Приватні канали можна ввімкнути в центрі адміністрування команд. Крім того, зверніть увагу, що, хоча зберігання приватних повідомлень каналу не підтримується, підтримується збереження файлів, що розподіляються в приватних каналах.

**Потрібен новий власник команди?**

Якщо власник приватного каналу залишає, ви можете додати нового власника команди за допомогою команди PowerShell.


- Відразу [тут](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , щоб встановити teams PowerShell.

Ось командлет вам буде потрібно:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Щоб отримати додаткові відомості про teams [PowerShell див.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)
