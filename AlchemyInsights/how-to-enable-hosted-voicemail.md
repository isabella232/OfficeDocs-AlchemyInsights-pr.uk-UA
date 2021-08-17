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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055575"
---
# <a name="how-to-enable-hosted-voicemail"></a>Увімкнення розміщеної голосової пошти

Щоб увімкнути голосову пошти, потрібно встановити значення **HostedVoicemail** $true.

**Властивість HostedVoicemail** для користувача, який використовує remote PowerShell (RPS).

Докладні відомості про підключення до запитів на Microsoft Teams [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) див. в цьому Microsoft Teams.

1. Адміністратор Teams ввійти у віддалену оболонку PowerShell для Teams.
1. З командного рядка PowerShell Teams адміністратор може запустити **set-csuser user@contoso.com -HostedVoiceMail $true** де sip uri має відповідного користувача.

> [!NOTE]
> Щоб реплікувати зміни до політик, може сягати 24 годин.