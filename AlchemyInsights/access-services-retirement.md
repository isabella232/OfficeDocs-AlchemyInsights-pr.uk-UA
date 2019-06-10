---
title: Доступ до послуг виходу на пенсію
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: f5a1e88e4443fdf43cdd4f07cf9e784810df7540
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34769489"
---
# <a name="access-services-retirement"></a><span data-ttu-id="57f1d-102">Доступ до послуг виходу на пенсію</span><span class="sxs-lookup"><span data-stu-id="57f1d-102">Access services retirement</span></span>

<span data-ttu-id="57f1d-103">Як ми спочатку оголошено в MC97576, в березні 2017 році і продовжив спілкуватися в минулому році послуги доступу є знаходяться у стані припинення зі служби Office 365.</span><span class="sxs-lookup"><span data-stu-id="57f1d-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="57f1d-104">Наступний етап у цьому процесі буде видалення доступу веб-бази даних, що використовують як їх основні зберігання даних списків SharePoint.</span><span class="sxs-lookup"><span data-stu-id="57f1d-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="57f1d-105">**Як це впливає на мене?**</span><span class="sxs-lookup"><span data-stu-id="57f1d-105">**How does this affect me?**</span></span>

<span data-ttu-id="57f1d-106">Починаючи з червня 2019, ми будемо Зупиніть створення нових баз даних Access у SharePoint Online і закриття послуги і всі решта застосунки до 2020 року квітня.</span><span class="sxs-lookup"><span data-stu-id="57f1d-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="57f1d-107">**Що мені потрібно зробити, щоб підготуватися до цієї зміни?**</span><span class="sxs-lookup"><span data-stu-id="57f1d-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="57f1d-108">Ми закликаємо вас створити план переходу для вашої організації веб-доступ до бази даних.</span><span class="sxs-lookup"><span data-stu-id="57f1d-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="57f1d-109">Адміністратори можна використовувати [застосунок SharePoint доступу сканера](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) для отримання інвентаризація доступ застосунків, які використовують сайти.</span><span class="sxs-lookup"><span data-stu-id="57f1d-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="57f1d-110">Існує кілька способів перенесення доступ до web баз даних:</span><span class="sxs-lookup"><span data-stu-id="57f1d-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="57f1d-111">Імпорт локальну базу даних Access (. ACCDB) або файл Excel.</span><span class="sxs-lookup"><span data-stu-id="57f1d-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="57f1d-112">Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативної платформи для створення бізнесу без коду рішень для веб- і мобільних пристроїв.</span><span class="sxs-lookup"><span data-stu-id="57f1d-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>