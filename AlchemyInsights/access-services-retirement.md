---
title: Пенсійні служби Access Services
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698703"
---
# <a name="access-services-retirement"></a><span data-ttu-id="67821-102">Пенсійні служби Access Services</span><span class="sxs-lookup"><span data-stu-id="67821-102">Access services retirement</span></span>

<span data-ttu-id="67821-103">Як ми спочатку анонсували в MC97576, у березні 2017, і продовжували спілкуватися за минулий рік, служби доступу в минулому році перебувають у відставку.</span><span class="sxs-lookup"><span data-stu-id="67821-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="67821-104">Наступний етап у цьому процесі стане видаленням веб-баз даних Access, які використовують списки SharePoint, як їх основний простір.</span><span class="sxs-lookup"><span data-stu-id="67821-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="67821-105">**Як це вплине на мене?**</span><span class="sxs-lookup"><span data-stu-id="67821-105">**How does this affect me?**</span></span>

<span data-ttu-id="67821-106">Починаючи з червня 2019, ми припиняємо створення нових баз даних Access у службі SharePoint Online і вимкніть службу та решту програм у квітні 2020.</span><span class="sxs-lookup"><span data-stu-id="67821-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="67821-107">**Що потрібно зробити, щоб підготуватися до цієї зміни?**</span><span class="sxs-lookup"><span data-stu-id="67821-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="67821-108">Радимо створити план переходу для веб-баз даних організації Access.</span><span class="sxs-lookup"><span data-stu-id="67821-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="67821-109">Адміністратори можуть використовувати [сканер програми SharePoint Access](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , щоб отримати інвентаризацію програм Access, які використовують сайти.</span><span class="sxs-lookup"><span data-stu-id="67821-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="67821-110">Перенести дані веб-баз даних Access можна кількома способами:</span><span class="sxs-lookup"><span data-stu-id="67821-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="67821-111">Імпорт до локальної бази даних Access (. ACCDB) або файл Excel.</span><span class="sxs-lookup"><span data-stu-id="67821-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="67821-112">Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативну платформу для створення без коду бізнес-рішень для веб-і мобільних пристроїв.</span><span class="sxs-lookup"><span data-stu-id="67821-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>