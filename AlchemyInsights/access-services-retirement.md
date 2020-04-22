---
title: Доступ до послуг виходу на пенсію
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687279"
---
# <a name="access-services-retirement"></a><span data-ttu-id="35655-102">Доступ до послуг виходу на пенсію</span><span class="sxs-lookup"><span data-stu-id="35655-102">Access services retirement</span></span>

<span data-ttu-id="35655-103">Як ми спочатку оголосили в MC97576, в березні 2017, і продовжував спілкуватися за минулий рік послуги доступу в даний час вийшли на пенсію.</span><span class="sxs-lookup"><span data-stu-id="35655-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="35655-104">Наступним етапом у цьому процесі буде видалення веб-баз даних Access, які використовують списки SharePoint як основне сховище даних.</span><span class="sxs-lookup"><span data-stu-id="35655-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="35655-105">**Як це впливає на мене?**</span><span class="sxs-lookup"><span data-stu-id="35655-105">**How does this affect me?**</span></span>

<span data-ttu-id="35655-106">Починаючи з червня 2019, ми зупиняємо створення нових баз даних Access у SharePoint Online і закрили службу та інші додатки до квітня 2020.</span><span class="sxs-lookup"><span data-stu-id="35655-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="35655-107">**Що потрібно зробити, щоб підготуватися до цієї зміни?**</span><span class="sxs-lookup"><span data-stu-id="35655-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="35655-108">Радимо створити план переходу для веб-баз даних Access вашої організації.</span><span class="sxs-lookup"><span data-stu-id="35655-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="35655-109">Адміністратори можуть використовувати [сканер застосунку SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для отримання інвентаризації програм Access, які використовують сайти.</span><span class="sxs-lookup"><span data-stu-id="35655-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="35655-110">Існує кілька способів перенести дані веб-баз даних Access:</span><span class="sxs-lookup"><span data-stu-id="35655-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="35655-111">Імпорт до бази даних локальних Access (. ACCDB) або до файлу Excel.</span><span class="sxs-lookup"><span data-stu-id="35655-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="35655-112">Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативну платформу для створення не-коду бізнес-рішень для веб-і мобільних пристроїв.</span><span class="sxs-lookup"><span data-stu-id="35655-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>