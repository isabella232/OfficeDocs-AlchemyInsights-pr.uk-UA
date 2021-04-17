---
title: Параметри політики нарад
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825464"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="90e76-102">Керування політиками нарад у Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="90e76-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="90e76-103">**Примітка. Зміни політики набирають сили для користувачів протягом 24 годин.**</span><span class="sxs-lookup"><span data-stu-id="90e76-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="90e76-104">Можливо, ви не зможете вносити зміни відразу до ново створених політик. зачекайте 4 години та спробуйте знову змінити щойно створену політику.</span><span class="sxs-lookup"><span data-stu-id="90e76-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="90e76-105">Політики нарад використовуються, щоб контролювати функції, доступні учасникам наради для нарад, які запланували користувачі у вашій організації.</span><span class="sxs-lookup"><span data-stu-id="90e76-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="90e76-106">Деякі функції політик нарад можуть ще не впроваджуватись у Центрі адміністрування Teams (вони позначені як "незабаром" у документації).</span><span class="sxs-lookup"><span data-stu-id="90e76-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="90e76-107">У цьому випадку або якщо з'являється таке повідомлення про помилку, як "Не вдалося оновити політику зараз, але повторити спробу пізніше" в Центрі адміністрування Microsoft Teams, радимо створити або змінити політики нарад Teams за допомогою PowerShell.</span><span class="sxs-lookup"><span data-stu-id="90e76-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="90e76-108">Докладні відомості про політики нарад див. в таких ресурсах:</span><span class="sxs-lookup"><span data-stu-id="90e76-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="90e76-109">Докладні відомості про створення політик, внесення змін і призначення користувачів політиці див. в розділі Керування [політиками нарад у Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="90e76-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="90e76-110">Відомості про змінення політики за допомогою командлетів PowerShell див. в [цьому огляді.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="90e76-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="90e76-111">Потрібно використовувати модуль [PowerShell "Skype для бізнесу" для](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) політик нарад Teams.</span><span class="sxs-lookup"><span data-stu-id="90e76-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="90e76-112">Докладні відомості див. в документації про командлети [\*-CsTeamsMeetingPolicy.](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="90e76-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

