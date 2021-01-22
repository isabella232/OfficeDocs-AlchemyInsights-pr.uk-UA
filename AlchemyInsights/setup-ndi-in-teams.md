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
# <a name="turn-on-ndi-technology"></a>Увімкнення технології NDI

Технологія NDI вимагає, щоб можна було ввімкнути два кроки для користувача.

1. Адміністратор клієнта має активувати властивість "Alowndistreaming" в політиці Cstefietingpolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Після того як ця зміна заповнюється, кінцевий користувач повинен ввімкнути технологію NDI® для певного клієнта з **настройок > дозволів**.

Докладні відомості наведено в статті [використання технології NDI в командах Microsoft](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings).
