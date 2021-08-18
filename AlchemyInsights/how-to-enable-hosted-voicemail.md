---
title: Увімкнення розміщеної голосової пошти
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318669"
---
# <a name="how-to-enable-hosted-voicemail"></a>Увімкнення розміщеної голосової пошти

Щоб увімкнути голосову пошти, потрібно встановити для **параметра HostedVoicemail** $true.

**Властивість HostedVoicemail** для користувача, який використовує remote PowerShell (RPS).

Докладні відомості про підключення до RPS див. в [Microsoft Teams PowerShell– огляд PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)

1. Адміністратор Teams ввійти в Remote PowerShell для Teams.
1. З командного рядка PowerShell Teams адміністратор може запустити **set-csuser user@contoso.com -HostedVoiceMail $true** де sip uri має відповідного користувача.

**Примітка.** Зміни політик можуть реплікувати до 24 годин.