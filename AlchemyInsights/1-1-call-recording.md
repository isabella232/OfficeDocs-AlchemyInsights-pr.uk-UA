---
title: записування викликів за 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733870"
---
# <a name="11-call-recording"></a>записування викликів за 1:1

Адміністраторам потрібно вжити заходів, щоб продовжити користувачам записувати виклики 1:1.
 
Починаючи з 12 квітня 2021, ми почнемо застосування нової політики виклику команд *AllowCloudRecordingForCalls*. 

Наразі функції *AllowCloudRecording* для записування викликів під 1:1 час наради в групах. Якщо користувачам дозволено записувати наради в групах, вони також можуть записувати виклики 1:1.

Якщо ви віддаєте перевагу блокувати всіх користувачів від записування викликів 1:1, не потрібно виконувати жодних дій. Параметр політики виклику *AllowCloudRecordingForCalls* буде $false за замовчуванням.

Ця зміна документована в наведеному нижче записі центру повідомлень: [(оновлено) 1:1 запис політики записування викликів](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) , щоб установити параметр політики викликів для команд, які потрібно використовувати як [PowerShell у групах](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Увімкнення запису викликів у службі 1:1:** Set-CsTeamsCallingPolicy – глобальний AllowCloudRecordingForCalls $True

**Щоб вимкнути записування викликів у службі 1:1, виконайте такі дії:** Set-CsTeamsCallingPolicy – глобальний AllowCloudRecordingForCalls $false

