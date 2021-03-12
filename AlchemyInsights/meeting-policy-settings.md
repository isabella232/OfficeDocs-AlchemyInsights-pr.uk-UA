---
title: Параметри політики наради
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704627"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="f6137-102">Керування політиками нарад у групах Microsoft</span><span class="sxs-lookup"><span data-stu-id="f6137-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="f6137-103">**Примітка. у разі внесення змін до політики для користувачів може знадобитися до 24 годин.**</span><span class="sxs-lookup"><span data-stu-id="f6137-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="f6137-104">Можливо, ви не зможете вносити зміни до щойно створених політик негайно; Зачекайте 4 години та спробуйте змінити щойно створену політику ще раз.</span><span class="sxs-lookup"><span data-stu-id="f6137-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="f6137-105">Політики нарад використовуються для керування функціями, доступними для учасників наради, запланованими користувачами в організації.</span><span class="sxs-lookup"><span data-stu-id="f6137-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="f6137-106">Деякі функції політик нарад, можливо, не реалізуються в центрі адміністрування команд, але ще (ці дані позначено як "Coming Soon" у документації).</span><span class="sxs-lookup"><span data-stu-id="f6137-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="f6137-107">У цьому випадку або якщо з'являється повідомлення про помилку "не вдалося оновити політику зараз, але повторіть спробу пізніше" в центрі адміністрування груп Microsoft, радимо використовувати PowerShell для створення або змінення політик нарад груп.</span><span class="sxs-lookup"><span data-stu-id="f6137-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="f6137-108">Щоб отримати докладні відомості про політики наради, ознайомтеся з такими ресурсами:</span><span class="sxs-lookup"><span data-stu-id="f6137-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="f6137-109">Щоб дізнатися про те, як створювати політики, вносити зміни та призначати користувачам політику, перегляньте статтю [керування політиками нарад в командах](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="f6137-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="f6137-110">Щоб внести зміни до політики за допомогою командлетів PowerShell, перегляньте статтю [Огляд PowerShell у групах](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="f6137-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="f6137-111">Потрібно використовувати [модуль "Skype для бізнесу PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) " для нарад у групах.</span><span class="sxs-lookup"><span data-stu-id="f6137-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="f6137-112">Перегляньте документацію за допомогою [командлетів \*-cstefietingpolicy](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) , щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="f6137-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

