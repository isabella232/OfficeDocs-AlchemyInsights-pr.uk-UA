---
title: Увімкнення пристрою
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
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256989"
---
# <a name="enable-device"></a>Увімкнення пристрою

**Активація пристрою за допомогою команди PowerShell**

Виконайте такі команди:

- Щоб отримати об'єкт пристрою, виконайте наведені нижче дії. `Get-MsolDevice -Name <Name>`
- Щоб увімкнути пристрій, виконайте наведені нижче дії. `Enable-MsolDevice -DeviceId <DeviceId>`

Докладні відомості про настроювання гібридного об'єднання в керованих доменах наведено в статті [Настроювання гібридного об'єднання](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).
