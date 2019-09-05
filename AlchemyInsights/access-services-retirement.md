---
title: Доступ до послуг виходу на пенсію
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 197366882468ebc87fc26f2fe2733371790d1871
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36747809"
---
# <a name="access-services-retirement"></a><span data-ttu-id="485e9-102">Доступ до послуг виходу на пенсію</span><span class="sxs-lookup"><span data-stu-id="485e9-102">Access services retirement</span></span>

<span data-ttu-id="485e9-103">Як ми спочатку оголосили в MC97576, в березні 2017, і продовжував спілкуватися за минулий рік служби доступу в даний час вийшли з офісу 365.</span><span class="sxs-lookup"><span data-stu-id="485e9-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="485e9-104">Наступним етапом у цьому процесі буде видалення веб-баз даних Access, які використовують списки SharePoint як основне сховище даних.</span><span class="sxs-lookup"><span data-stu-id="485e9-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="485e9-105">**Як це впливає на мене?**</span><span class="sxs-lookup"><span data-stu-id="485e9-105">**How does this affect me?**</span></span>

<span data-ttu-id="485e9-106">Починаючи з червня 2019, ми зупиняємо створення нових баз даних Access у SharePoint Online і закрили службу та інші додатки до квітня 2020.</span><span class="sxs-lookup"><span data-stu-id="485e9-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="485e9-107">**Що потрібно зробити, щоб підготуватися до цієї зміни?**</span><span class="sxs-lookup"><span data-stu-id="485e9-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="485e9-108">Радимо створити план переходу для веб-баз даних Access вашої організації.</span><span class="sxs-lookup"><span data-stu-id="485e9-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="485e9-109">Адміністратори можуть використовувати [сканер застосунку SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для отримання інвентаризації програм Access, які використовують сайти.</span><span class="sxs-lookup"><span data-stu-id="485e9-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="485e9-110">Існує кілька способів перенести дані веб-баз даних Access:</span><span class="sxs-lookup"><span data-stu-id="485e9-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="485e9-111">Імпорт до бази даних локальних Access (. ACCDB) або до файлу Excel.</span><span class="sxs-lookup"><span data-stu-id="485e9-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="485e9-112">Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативну платформу для створення не-коду бізнес-рішень для веб-і мобільних пристроїв.</span><span class="sxs-lookup"><span data-stu-id="485e9-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>