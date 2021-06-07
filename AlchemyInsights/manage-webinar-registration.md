---
title: Керування реєстрацією веб-inарів
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
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794142"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="882a5-102">Керування реєстрацією веб-inарів</span><span class="sxs-lookup"><span data-stu-id="882a5-102">Manage webinar registration</span></span>

<span data-ttu-id="882a5-103">Ви можете керувати списком користувачів, які Teams вебінарів, використовуючи Teams команд PowerShell.</span><span class="sxs-lookup"><span data-stu-id="882a5-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="882a5-104">Відомості про те Teams, як інсталювати PowerShell, [Teams PowerShell.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="882a5-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="882a5-105">За замовчуванням *параметр WhoCanRegister* увімкнуто та встановлено значення **EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="882a5-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="882a5-106">Щоб дозволити реєструвати всіх користувачів, зокрема анонімних користувачів, потрібно вибрати для параметра Політика наради значення **Усі** за допомогою команди PowerShell:</span><span class="sxs-lookup"><span data-stu-id="882a5-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="882a5-107">**Примітка.** Якщо анонімне приєднання вимкнуто в параметрах наради, анонімні користувачі не можуть приєднатися до вебінарів.</span><span class="sxs-lookup"><span data-stu-id="882a5-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="882a5-108">Докладні відомості та ввімкнення цієї настройки див. в розділі [Керування параметрами наради Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span><span class="sxs-lookup"><span data-stu-id="882a5-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="882a5-109">Щоб вимкнути реєстрацію наради, установіть для параметра *AllowMeetingRegistration значення* **False (Хибість).**</span><span class="sxs-lookup"><span data-stu-id="882a5-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="882a5-110">Докладні відомості про настроювання користувачів, які можуть зареєструватися для вебінарів, див. в статтях Настроювання користувачів, які [можуть зареєструватися для вебінарів.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="882a5-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="882a5-111">Докладні відомості про параметри для microsoft Lists див. в [статті Параметри керування для Microsoft Lists.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="882a5-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
