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
# <a name="private-channels-in-microsoft-teams"></a><span data-ttu-id="3f63b-102">Приватні канали у Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="3f63b-102">Private channels in Microsoft Teams</span></span>

<span data-ttu-id="3f63b-103">Приватні канали – це нова функція у Microsoft teams.</span><span class="sxs-lookup"><span data-stu-id="3f63b-103">Private channels is a new feature in Microsoft Teams.</span></span> <span data-ttu-id="3f63b-104">Зауважте, що приватні канали не можна конвертувати зі стандартних каналів або навпаки.</span><span class="sxs-lookup"><span data-stu-id="3f63b-104">Note that private channels cannot be converted from standard channels or vice versa.</span></span>

<span data-ttu-id="3f63b-105">Щоб отримати докладні відомості про приватні канали, такі як інформація про [створення приватних каналів і членство](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) та [приватний канал SharePoint сайтів](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), перегляньте [приватні канали в Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span><span class="sxs-lookup"><span data-stu-id="3f63b-105">For details about private channels, such as information on [private channel creation and membership](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) and [private channel SharePoint sites](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), see [Private channels in Microsoft Teams](https://docs.microsoft.com/MicrosoftTeams/private-channels).</span></span> 

<span data-ttu-id="3f63b-106">**Примітка:** Оскільки конфігурація для збереження повідомлень приватного каналу ще не підтримується, орендарі з увімкнутими політиками збереження не матимуть приватних каналів, увімкнуті за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="3f63b-106">**Note:** Because configuration for retention of private channel messages is not yet supported, tenants with retention policies enabled will not have private channels enabled by default.</span></span> <span data-ttu-id="3f63b-107">Приватні канали можна ввімкнути в центрі адміністрування команд.</span><span class="sxs-lookup"><span data-stu-id="3f63b-107">Private channels can be enabled in the Teams admin center.</span></span> <span data-ttu-id="3f63b-108">Крім того, зверніть увагу, що, хоча зберігання приватних повідомлень каналу не підтримується, підтримується збереження файлів, що розподіляються в приватних каналах.</span><span class="sxs-lookup"><span data-stu-id="3f63b-108">Also, note that while retention of private channel messages is not supported, retention of files shared in private channels is supported.</span></span>

<span data-ttu-id="3f63b-109">**Потрібен новий власник команди?**</span><span class="sxs-lookup"><span data-stu-id="3f63b-109">**Need a new team owner?**</span></span>

<span data-ttu-id="3f63b-110">Якщо власник приватного каналу залишає, ви можете додати нового власника команди за допомогою команди PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3f63b-110">If your private channel owner leaves, you can add a new team owner via Teams Powershell.</span></span>


- <span data-ttu-id="3f63b-111">Відразу [тут](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) , щоб встановити teams PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3f63b-111">Go [here](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) to install Teams Powershell.</span></span>

<span data-ttu-id="3f63b-112">Ось командлет вам буде потрібно:</span><span class="sxs-lookup"><span data-stu-id="3f63b-112">Here is the cmdlet you will need:</span></span>

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

<span data-ttu-id="3f63b-113">Щоб отримати додаткові відомості про teams [PowerShell див.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="3f63b-113">For more information on Teams Powershell, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span>
