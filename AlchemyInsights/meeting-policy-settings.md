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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042865"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="86e8d-102">Керування політиками нарад у Microsoft teams</span><span class="sxs-lookup"><span data-stu-id="86e8d-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="86e8d-103">**Примітка: це може зайняти до 24 годин, щоб зміни політики набрали сили для користувачів.**</span><span class="sxs-lookup"><span data-stu-id="86e8d-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="86e8d-104">Ви не зможете негайно вносити зміни до щойно створених політик; Зачекайте 4 години та спробуйте змінити знову створену політику.</span><span class="sxs-lookup"><span data-stu-id="86e8d-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="86e8d-105">Політика для нарад використовується для керування функціями, доступними для учасників нарад, запланованих користувачами в організації.</span><span class="sxs-lookup"><span data-stu-id="86e8d-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="86e8d-106">Деякі функції політики нарад можуть не реалізовуватися в центрі адміністрування команд (ці дані позначено як "скоро" у документації).</span><span class="sxs-lookup"><span data-stu-id="86e8d-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="86e8d-107">У цьому випадку, або якщо ви отримуєте повідомлення про помилку "ми не можемо оновити політику прямо зараз, але повторіть спробу пізніше" у центр адміністрування Microsoft teams, рекомендовано використовувати PowerShell для створення або змінення політики для нарад, teams.</span><span class="sxs-lookup"><span data-stu-id="86e8d-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="86e8d-108">Додаткові відомості про правила для нарад можна отримати в таких ресурсах:</span><span class="sxs-lookup"><span data-stu-id="86e8d-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="86e8d-109">Щоб дізнатися про створення політик, внесення змін і призначення користувачів політиці [, див.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="86e8d-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="86e8d-110">Щоб внести зміни до політики за допомогою командлети PowerShell [, див.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="86e8d-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="86e8d-111">Потрібно використовувати [Skype, бізнес-PowerShell модуль](https://www.microsoft.com/download/details.aspx?id=39366) для робочих груп, наради політики.</span><span class="sxs-lookup"><span data-stu-id="86e8d-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="86e8d-112">Перегляньте [документацію \*-cпаросletingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) для отримання додаткових відомостей</span><span class="sxs-lookup"><span data-stu-id="86e8d-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

