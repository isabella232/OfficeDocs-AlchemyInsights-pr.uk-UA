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
ms.openlocfilehash: ed932592aae1158bc0c0da4817467b69d20208533bc080cb0e424f552af8601a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023543"
---
# <a name="turn-on-ndi-technology"></a>Увімкнення технології NDI

Щоб активувати технологію NDI для користувача, потрібно виконати два кроки:

1. Адміністратор клієнта має активувати властивість AllowNDIStreaming у CsTeamsMeetingPolicy.

    `Set-CsTeamsMeetingPolicy -Identity MEETING_POLICY -AllowNDIStreaming $true`

2. Після заповнення цієї зміни користувач має активувати технологію NDI® для певного клієнта з **Настройки > Дозволи.**

Докладні відомості див. в [цій Microsoft Teams.](https://docs.microsoft.com/microsoftteams/use-ndi-in-meetings)
