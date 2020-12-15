---
title: Увімкнення розміщення голосової пошти
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679161"
---
# <a name="how-to-enable-hosted-voicemail"></a>Увімкнення розміщення голосової пошти

Щоб активувати голосову пошту, потрібно настроїти **голосову пошту** на $True.

Властивість **Hostedvoicemail пошта** користувача за допомогою віддаленого PowerShell (RPS).

Щоб отримати докладніші відомості про підключення до RPS, ознайомтеся з додатковими відомостями про підключення до RPS у [програмі Microsoft](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) .

1. Адміністратор команди має увійти в віддалений PowerShell для команд.
1. У програмі PowerShell запит адміністратор команди може запустити **Set-csuser user@contoso.com-HostedVoiceMail пошта $True** , де SIP URI має користувача в питанні.

> [!NOTE]
> Зміни в політиці можуть знадобитися до 24 годин, щоб реплікувати.