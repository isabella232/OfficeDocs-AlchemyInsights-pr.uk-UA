---
title: Увімкнення Teams вебінарів
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794035"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="e4c93-102">Увімкнення Teams вебінарів</span><span class="sxs-lookup"><span data-stu-id="e4c93-102">Enable Teams Webinars</span></span>

<span data-ttu-id="e4c93-103">Вебінари ввімкнуто за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="e4c93-103">Webinars are enabled by default.</span></span> <span data-ttu-id="e4c93-104">За допомогою команд PowerShell можна впорядковувати та Teams Teams для вебінарів.</span><span class="sxs-lookup"><span data-stu-id="e4c93-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="e4c93-105">Усі користувачі, які можуть створити нараду, також можуть створювати веб-наради.</span><span class="sxs-lookup"><span data-stu-id="e4c93-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="e4c93-106">Щоб керувати списком користувачів, які можуть планувати Teams, використовуйте *параметр AllowMeetingRegistration.*</span><span class="sxs-lookup"><span data-stu-id="e4c93-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="e4c93-107">За замовчуванням *параметр WhoCanRegister* увімкнуто та встановлено значення **Усі.**</span><span class="sxs-lookup"><span data-stu-id="e4c93-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="e4c93-108">Щоб вимкнути реєстрацію наради, установіть для параметра *AllowMeetingRegistration значення* **False (Хибість).**</span><span class="sxs-lookup"><span data-stu-id="e4c93-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="e4c93-109">Щоб змінити ці параметри, потрібно інсталювати Teams [PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="e4c93-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="e4c93-110">Крім того, політики нарад застосовуються Teams вебінарів.</span><span class="sxs-lookup"><span data-stu-id="e4c93-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="e4c93-111">Наприклад, якщо анонімне приєднання вимкнуто в параметрах наради, анонімні користувачі не можуть приєднатися до вебінарів.</span><span class="sxs-lookup"><span data-stu-id="e4c93-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="e4c93-112">Докладні відомості про настроювання користувачів, які можуть зареєструватися для вебінарів, див. в статтях Настроювання користувачів, які [можуть зареєструватися для вебінарів.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="e4c93-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="e4c93-113">Докладні відомості про параметри для microsoft Lists див. в [статті Параметри керування для Microsoft Lists.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="e4c93-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>