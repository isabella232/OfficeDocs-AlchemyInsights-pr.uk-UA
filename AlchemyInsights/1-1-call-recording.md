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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702111"
---
# <a name="11-call-recording"></a><span data-ttu-id="db396-102">Запис викликів: 1:1</span><span class="sxs-lookup"><span data-stu-id="db396-102">1:1 call recording</span></span>

<span data-ttu-id="db396-103">Якщо кнопка **Почати записування** неясна під час виклику о 1:1, потрібно змінити параметри політики для потрібного користувача.</span><span class="sxs-lookup"><span data-stu-id="db396-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="db396-104">Щоб перевірити параметр політики, запустіть діагностичну для цього користувача, ввівши вище **параметр Diag: Teams 1:1 Call Recording** (Записування викликів).</span><span class="sxs-lookup"><span data-stu-id="db396-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="db396-105">З 31 травня 202 Teams 1 року ми почнемо застосовувати нову політику викликів *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="db396-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="db396-106">До цієї зміни записування викликів о 1:1 контролюється політикою нарад *AllowCloudRecording Teams* нарад.</span><span class="sxs-lookup"><span data-stu-id="db396-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="db396-107">Ця зміна документується в дописі в Центрі повідомлень: [(Оновлено) 1:1 Вступ до політики записування викликів](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span><span class="sxs-lookup"><span data-stu-id="db396-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="db396-108">*AllowCloudRecordingForCalls*   Параметр "Політика викликів" установлено **$False** за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="db396-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="db396-109">Щоб заборонити всім користувачам записувати виклики "о 1:1", нічого робити не потрібно.</span><span class="sxs-lookup"><span data-stu-id="db396-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="db396-110">Щоб увімкнути записування викликів для всіх користувачів в цілодобовому оболонці [Teams PowerShell](/microsoftteams/teams-powershell-install) виконати такий командлет:</span><span class="sxs-lookup"><span data-stu-id="db396-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="db396-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="db396-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="db396-112">Крім того, ви можете створити політику та вибрати **параметр -AllowCloudRecordingForCalls** $true призначити цю політику користувачам. </span><span class="sxs-lookup"><span data-stu-id="db396-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="db396-113">Докладні відомості див. в дописі 1:1 Елементи керування політикою записування [викликів (майже!) Тут](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="db396-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
