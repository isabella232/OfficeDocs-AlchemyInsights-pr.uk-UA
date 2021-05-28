---
title: 'Запис викликів: 1:1'
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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696979"
---
# <a name="11-call-recording"></a><span data-ttu-id="83c5d-102">Запис викликів: 1:1</span><span class="sxs-lookup"><span data-stu-id="83c5d-102">1:1 call recording</span></span>

<span data-ttu-id="83c5d-103">Якщо кнопка **Почати записування** неясна під час виклику о 1:1, потрібно змінити параметри політики для потрібного користувача.</span><span class="sxs-lookup"><span data-stu-id="83c5d-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="83c5d-104">З 31 травня 202 Teams 1 року ми почнемо застосовувати нову політику викликів *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="83c5d-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="83c5d-105">До цієї зміни записування викликів о 1:1 контролюється політикою нарад *AllowCloudRecording Teams* нарад.</span><span class="sxs-lookup"><span data-stu-id="83c5d-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="83c5d-106">Ця зміна документується в дописі в Центрі повідомлень: [(Оновлено) 1:1 Вступ до політики записування викликів](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="83c5d-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="83c5d-107">*AllowCloudRecordingForCalls*   Параметр "Політика викликів" установлено **$False** за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="83c5d-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="83c5d-108">Щоб заборонити всім користувачам записувати виклики "о 1:1", нічого робити не потрібно.</span><span class="sxs-lookup"><span data-stu-id="83c5d-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="83c5d-109">Щоб увімкнути записування викликів для всіх користувачів в обидві особи, виконайте цей командлет Teams PowerShell:</span><span class="sxs-lookup"><span data-stu-id="83c5d-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="83c5d-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="83c5d-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="83c5d-111">Крім того, ви можете створити політику та вибрати **параметр -AllowCloudRecordingForCalls** $true призначити цю політику користувачам. </span><span class="sxs-lookup"><span data-stu-id="83c5d-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="83c5d-112">Докладні відомості див. в дописі 1:1 Елементи керування політикою записування [викликів (майже!) Тут](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="83c5d-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
