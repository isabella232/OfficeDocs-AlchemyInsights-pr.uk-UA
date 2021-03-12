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
# <a name="11-call-recording"></a><span data-ttu-id="2a082-102">записування викликів за 1:1</span><span class="sxs-lookup"><span data-stu-id="2a082-102">1:1 call recording</span></span>

<span data-ttu-id="2a082-103">Адміністраторам потрібно вжити заходів, щоб продовжити користувачам записувати виклики 1:1.</span><span class="sxs-lookup"><span data-stu-id="2a082-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="2a082-104">Починаючи з 12 квітня 2021, ми почнемо застосування нової політики виклику команд *AllowCloudRecordingForCalls*.</span><span class="sxs-lookup"><span data-stu-id="2a082-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="2a082-105">Наразі функції *AllowCloudRecording* для записування викликів під 1:1 час наради в групах.</span><span class="sxs-lookup"><span data-stu-id="2a082-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="2a082-106">Якщо користувачам дозволено записувати наради в групах, вони також можуть записувати виклики 1:1.</span><span class="sxs-lookup"><span data-stu-id="2a082-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="2a082-107">Якщо ви віддаєте перевагу блокувати всіх користувачів від записування викликів 1:1, не потрібно виконувати жодних дій.</span><span class="sxs-lookup"><span data-stu-id="2a082-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="2a082-108">Параметр політики виклику *AllowCloudRecordingForCalls* буде $false за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="2a082-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="2a082-109">Ця зміна документована в наведеному нижче записі центру повідомлень: [(оновлено) 1:1 запис політики записування викликів](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) , щоб установити параметр політики викликів для команд, які потрібно використовувати як [PowerShell у групах](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="2a082-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="2a082-110">**Увімкнення запису викликів у службі 1:1:** Set-CsTeamsCallingPolicy – глобальний AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="2a082-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="2a082-111">**Щоб вимкнути записування викликів у службі 1:1, виконайте такі дії:** Set-CsTeamsCallingPolicy – глобальний AllowCloudRecordingForCalls $false</span><span class="sxs-lookup"><span data-stu-id="2a082-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

