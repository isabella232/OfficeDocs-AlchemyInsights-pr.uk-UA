---
title: Увімкнення технології NDI
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004403"
- "7947"
ms.openlocfilehash: ea694898baffa50fca71957175eba3664dece44e
ms.sourcegitcommit: 112f18dce8257b98fab32d44910ee879efb44cb8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935197"
---
# <a name="turn-on-ndi-technology"></a><span data-ttu-id="a13df-102">Увімкнення технології NDI</span><span class="sxs-lookup"><span data-stu-id="a13df-102">Turn on NDI technology</span></span>

<span data-ttu-id="a13df-103">Технологія NDI вимагає, щоб можна було ввімкнути два кроки для користувача.</span><span class="sxs-lookup"><span data-stu-id="a13df-103">NDI technology requires two steps to be turned on for a user:</span></span>

1. <span data-ttu-id="a13df-104">Адміністратор клієнта має активувати властивість "Alowndistreaming" в політиці Cstefietingpolicy.</span><span class="sxs-lookup"><span data-stu-id="a13df-104">The tenant admin must enable the 'AllowNDIStreaming' property in CsTeamsMeetingPolicy.</span></span>

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. <span data-ttu-id="a13df-105">Після того як ця зміна заповнюється, кінцевий користувач повинен ввімкнути технологію NDI® для певного клієнта з **настройок > дозволів**.</span><span class="sxs-lookup"><span data-stu-id="a13df-105">After this change has populated, the end user must turn on NDI® technology for their specific client from **Settings > Permissions**.</span></span>

<span data-ttu-id="a13df-106">Докладні відомості наведено в статті [використання технології NDI в командах Microsoft](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span><span class="sxs-lookup"><span data-stu-id="a13df-106">For more information, see [Use NDI technology in Microsoft Teams](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).</span></span>
