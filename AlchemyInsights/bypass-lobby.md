---
title: Обхід лобі
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684971"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="5bdb2-102">Керування параметрами лобі та рівнем участі в командах</span><span class="sxs-lookup"><span data-stu-id="5bdb2-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="5bdb2-103">Щоб дозволити всім, зокрема використовувати комутоване, зовнішні та анонімні користувачі, щоб **обійти фойє**, використовуйте PowerShell, щоб виконати це завдання.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="5bdb2-104">Нижче наведено приклад змінення політики глобального наради для вашої організації.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="5bdb2-105">Цей командлет зараз вимагає використання модуля "Skype для бізнесу PowerShell".</span><span class="sxs-lookup"><span data-stu-id="5bdb2-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="5bdb2-106">Щоб налаштувати використання цього командлета, перегляньте [керування політиками за допомогою PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="5bdb2-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="5bdb2-107">Коли ви настроїли політику, потрібно використати її для користувачів; або, якщо ви змінили глобальну політику, вона автоматично застосуться до користувачів.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="5bdb2-108">Для будь-якої зміни політики потрібно зачекати щонайменше **4 години до 24 годин** , щоб політики набрали сили.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="5bdb2-109">Обов'язково ознайомтеся з документацією нижче, перш ніж вносити ці зміни, щоб точно розуміти, що це дозволяє.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="5bdb2-110">Загальні відомості про елементи керування "лобіювання політики" в командах нарад</span><span class="sxs-lookup"><span data-stu-id="5bdb2-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="5bdb2-111">Ці параметри керують тим, що Учасники наради очікують у фойє, перш ніж вони будуть допущені до наради, а рівень участі, яке їм дозволено під час наради.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="5bdb2-112">За допомогою PowerShell можна оновити настройки політики наради, які ще не реалізовано (з позначкою "Coming Soon") у центрі адміністрування команд.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="5bdb2-113">Нижче наведено приклад командлет PowerShell, який дає змогу всім користувачам обходити вестибюль.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="5bdb2-114">[Автоматично визнавати людей](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) – це політика для Організатора, яка керує тим, що користувачі можуть приєднатися до наради безпосередньо або чекати в холі, доки вони не будуть допущені автентифікованим користувачем.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="5bdb2-115">[Дозволити анонімним користувачам почати нараду](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) – це політика для Організатора, яка керує тим, що користувачі, зокрема B2B та федеративного користувачів, можуть приєднатися до наради користувача без автентифікованого користувача в організації.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="5bdb2-116">[Дозволити користувачам](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) , які не мають права на вхід у вестибюлі (**незабаром**) – це політика для Організатора, яка керує тим, що користувачі, які телефонають за допомогою телефону, можуть приєднатися до наради безпосередньо або чекати в холі, незалежно від того, чи **автоматично визнають користувачів** настройку.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="5bdb2-117">[Дозволити організаторам змінювати настройки лобі](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**незабаром**) – це політика для Організатора, яка керує тим, що Організатор наради може змінити настройки лобі, які настроєно адміністратором, щоб **автоматично визнавати** **користувачів і дозволити користувачам комутованого з них обходити вестибюль** під час планування нової наради.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="5bdb2-118">**Примітка.** Прочитайте [керування політиками нарад в командах](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) для повного огляду політик нарад Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5bdb2-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
