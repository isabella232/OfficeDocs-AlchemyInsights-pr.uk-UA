---
title: Параметри політики для нарад
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627595"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="750bf-102">Керування політиками нарад у Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="750bf-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="750bf-103">Політика для нарад використовується для керування функціями, доступними для учасників нарад, запланованих користувачами в організації.</span><span class="sxs-lookup"><span data-stu-id="750bf-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="750bf-104">Деякі функції політики нарад можуть не реалізовуватися в центрі адміністрування команд (ці дані позначено як "скоро" у документації).</span><span class="sxs-lookup"><span data-stu-id="750bf-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="750bf-105">У цьому випадку, або якщо ви отримуєте повідомлення про помилку "ми не можемо оновити політику прямо зараз, але повторіть спробу пізніше" у центр адміністрування Microsoft teams, рекомендовано використовувати PowerShell для створення або змінення політики для нарад, teams.</span><span class="sxs-lookup"><span data-stu-id="750bf-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="750bf-106">Додаткові відомості про правила для нарад можна отримати в таких ресурсах:</span><span class="sxs-lookup"><span data-stu-id="750bf-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="750bf-107">Щоб дізнатися про створення політик, внесення змін і призначення користувачів політиці [, див.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="750bf-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="750bf-108">Щоб внести зміни до політики за допомогою командлети PowerShell [, див.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="750bf-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="750bf-109">Потрібно використовувати [Skype, бізнес-PowerShell модуль](https://www.microsoft.com/download/details.aspx?id=39366) для робочих груп, наради політики.</span><span class="sxs-lookup"><span data-stu-id="750bf-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="750bf-110">Перегляньте [документацію \*-cпаросletingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) для отримання додаткових відомостей</span><span class="sxs-lookup"><span data-stu-id="750bf-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="750bf-111">**Примітка:** Зміни в політиці можуть тривати до 24 годин, щоб вони набрали сили для користувачів.</span><span class="sxs-lookup"><span data-stu-id="750bf-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="750bf-112">Ви не зможете негайно вносити зміни до щойно створених політик; Зачекайте 4 години та спробуйте змінити знову створену політику.</span><span class="sxs-lookup"><span data-stu-id="750bf-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="750bf-113">Якщо проблеми не виникають, спробуйте PowerShell.</span><span class="sxs-lookup"><span data-stu-id="750bf-113">If you're still having problems, try PowerShell.</span></span>  