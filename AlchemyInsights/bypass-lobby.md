---
title: Обійти фойє
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820055"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="9d0c1-102">Керування параметрами фойє та рівнем участі в Teams</span><span class="sxs-lookup"><span data-stu-id="9d0c1-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="9d0c1-103">Щоб обійти фойє, скористайтеся PowerShell, щоб виконати це завдання, якщо потрібно дозволити всім, зокрема вхідні, зовнішні та анонімні користувачі. </span><span class="sxs-lookup"><span data-stu-id="9d0c1-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="9d0c1-104">Ось приклад змінення глобальної політики наради для організації.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="9d0c1-105">Цей командлет наразі потребує використання модуля PowerShell служби "Skype для бізнесу".</span><span class="sxs-lookup"><span data-stu-id="9d0c1-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="9d0c1-106">Щоб налаштувати використання цього командлета, ознайомтесь із цією цією командлетом, щоб дізнатися про керування [політиками за допомогою PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="9d0c1-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="9d0c1-107">Після налаштування політики її потрібно застосувати до користувачів. або, якщо ви змінили політику Global, вона автоматично застосовуватиме до користувачів.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="9d0c1-108">Щоб політики набрали сили, зачекайте принаймні 4 години до **24** годин.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="9d0c1-109">Обов'язково перегляньте наведену нижче документацію, перш ніж вносити ці зміни, щоб зрозуміти, що це дозволяє.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="9d0c1-110">Докладні відомості про елементи керування політикою "фойє" наради Teams</span><span class="sxs-lookup"><span data-stu-id="9d0c1-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="9d0c1-111">Ці параметри керують тим, які учасники наради чекають у фойє, перш ніж їх буде прийнято на нараду, і рівень участі, які вони можуть брати на нараду.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="9d0c1-112">За допомогою PowerShell можна оновити параметри політики нарад, які ще не впроваджено (з позначкою "незабаром") у Центрі адміністрування Teams.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="9d0c1-113">Нижче наведено приклад командлета PowerShell, який дає змогу всім користувачам обійти фойє.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="9d0c1-114">[Автоматично допускати](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) користувачів – це політика кожного організатора, яка визначає, чи користувачі можуть безпосередньо приєднуватися до наради, або чекати у "фойє", доки автентифікований користувач не приєднається до наради.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="9d0c1-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Дозволити анонімним користувачам розпочинати нараду – це політика кожного організатора, яка визначає, чи можуть анонімні користувачі, зокрема B2B та федеративні користувачі, приєднатися до наради користувача без автентифікованого користувача з організації під час відвідування.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="9d0c1-116">Дозволити [користувачам-організаторам](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) обходити фойє **(очікується** незабаром) – це політика від кожного організатора, яка визначає, чи користувачі, які приєднаються  по телефону, можуть безпосередньо приєднатися до наради або чекати у фойє незалежно від параметра Автоматично допускати користувачів.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="9d0c1-117">Дозволити організаторам перевизначати настройки фойє (незабаром) – це політика кожного організатора, яка визначає, чи може  організатор наради  перевизначати параметри фойє, установлені адміністратором у розділі Автоматичне допускання користувачів і Надання користувачам дозволу оминати фойє під час планування нової наради. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) </span><span class="sxs-lookup"><span data-stu-id="9d0c1-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="9d0c1-118">**Примітка.** Повний [огляд політик нарад Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) див. в статті Керування політиками нарад у Teams.</span><span class="sxs-lookup"><span data-stu-id="9d0c1-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
