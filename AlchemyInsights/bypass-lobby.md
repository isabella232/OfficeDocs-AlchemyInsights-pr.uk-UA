---
title: Обійти лобі
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376897"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="eb70f-102">Контроль параметрів лобі та рівень участі</span><span class="sxs-lookup"><span data-stu-id="eb70f-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="eb70f-103">Ці настройки керують тим, що учасники зустрічі чекають у вестибюлі, перш ніж вони будуть допущені до зустрічі і рівень участі, який вони можуть отримати на нараді.</span><span class="sxs-lookup"><span data-stu-id="eb70f-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="eb70f-104">PowerShell можна використовувати для оновлення зустрічі параметри політики, які ще не реалізовано (з написом "скоро") у команди центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="eb70f-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="eb70f-105">Нижче наведено приклад командлета PowerShell, який дозволяє всім користувачам обходити фойє.</span><span class="sxs-lookup"><span data-stu-id="eb70f-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="eb70f-106">[Автоматично визнати](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , що люди в політиці для Організатора, що контролює, чи є люди приєднатися до наради безпосередньо або чекати у фойє, поки вони не будуть допущені автентифікованим користувачем.</span><span class="sxs-lookup"><span data-stu-id="eb70f-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="eb70f-107">[Дозволити анонімним людям розпочати нараду](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) – це політика Організатора, яка керує тим, чи можуть користувачі анонімних користувачів, ВКЛЮЧНО з B2B та федеративними користувачами, приєднатися до наради користувача без автентифікованого користувача з організації.</span><span class="sxs-lookup"><span data-stu-id="eb70f-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="eb70f-108">[Дозволити комутованого користувачів, щоб обійти фойє](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) є для Організатора політики, яка контролює, чи люди, які підключаються по телефону приєднатися до наради безпосередньо або чекати в холі, незалежно від того, **автоматично визнати, люди** налаштування.</span><span class="sxs-lookup"><span data-stu-id="eb70f-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="eb70f-109">[Дозволити організаторам змінювати параметри фойє](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**скоро**)-це політика Організатора, яка керує тим, чи може Організатор наради перевизначити настройки фойє, які встановлюються адміністратором у **автоматичному режимі** \*\* користувачі, щоб обійти фойє\*\* під час планування нової наради.</span><span class="sxs-lookup"><span data-stu-id="eb70f-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="eb70f-110">**Примітка:** Для повного огляду політики зборів Microsoft teams прочитайте [команди керування політикою нарад](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) .</span><span class="sxs-lookup"><span data-stu-id="eb70f-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="eb70f-111">**Приклад PowerShell**</span><span class="sxs-lookup"><span data-stu-id="eb70f-111">**PowerShell example**</span></span>

<span data-ttu-id="eb70f-112">Якщо ви хочете дозволити всім, включаючи зовнішніх або анонімних користувачів, обійти фойє, ви також можете використовувати PowerShell для виконання цього завдання.</span><span class="sxs-lookup"><span data-stu-id="eb70f-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="eb70f-113">Нижче наведено приклад змінення політики глобального наради для вашої організації.</span><span class="sxs-lookup"><span data-stu-id="eb70f-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="eb70f-114">(Обов'язково перегляньте документацію вище, перш ніж вносити ці зміни, щоб точно зрозуміти, що це дозволяє.)</span><span class="sxs-lookup"><span data-stu-id="eb70f-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="eb70f-115">Набір-Cпароплавполітика-ідентичність Global-AutoAdmittedUsers "все"-Дозволяєредагувати $True</span><span class="sxs-lookup"><span data-stu-id="eb70f-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="eb70f-116">Щоб отримати додаткові відомості, [див.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)</span><span class="sxs-lookup"><span data-stu-id="eb70f-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
