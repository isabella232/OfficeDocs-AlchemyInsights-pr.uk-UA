---
title: Видалення або виключення команд із пакета Office
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
- "2662"
- "9000660"
ms.openlocfilehash: 22d69db749671afdfe7a809d1bc598e2ad1891d8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658242"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="40e9d-102">Видалення або виключення команд із нових або поточних інсталяцій Office</span><span class="sxs-lookup"><span data-stu-id="40e9d-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="40e9d-103">Команди Microsoft входять до складу програм Microsoft 365 для підприємств, програм Microsoft 365 для бізнесу та Office для Mac.</span><span class="sxs-lookup"><span data-stu-id="40e9d-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="40e9d-104">Використовуйте [засіб розгортання Office](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) , щоб виключити команди з нових інсталяцій Office.</span><span class="sxs-lookup"><span data-stu-id="40e9d-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="40e9d-105">Щоб *Видалити* команди з пристрою під керуванням ОС Windows, перегляньте статтю [видалення команд Microsoft](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span><span class="sxs-lookup"><span data-stu-id="40e9d-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="40e9d-106">Щоб очистити групи Microsoft із кількох цільових машин або користувачів, ознайомтеся з командою [Microsoft розгортання команд](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span><span class="sxs-lookup"><span data-stu-id="40e9d-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="40e9d-107">За допомогою параметра [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) можна заборонити автоматичне інсталювання команд із програмою Office.</span><span class="sxs-lookup"><span data-stu-id="40e9d-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="40e9d-108">Скористайтеся параметром [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) , *перш ніж інсталювати команди*, щоб заборонити автоматичний запуск команд Microsoft після інсталяції.</span><span class="sxs-lookup"><span data-stu-id="40e9d-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="40e9d-109">Якщо ви використовуєте Office для Mac, ознайомтеся [з командами Microsoft для інсталяції на комп'ютері Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span><span class="sxs-lookup"><span data-stu-id="40e9d-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>