---
title: Доступ до послуг виходу на пенсію
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973960"
---
# <a name="access-services-retirement"></a><span data-ttu-id="0c501-102">Доступ до послуг виходу на пенсію</span><span class="sxs-lookup"><span data-stu-id="0c501-102">Access services retirement</span></span>

<span data-ttu-id="0c501-103">Як ми спочатку оголошено в MC97576, в березні 2017 році і продовжив спілкуватися в минулому році послуги доступу є знаходяться у стані припинення зі служби Office 365.</span><span class="sxs-lookup"><span data-stu-id="0c501-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="0c501-104">Наступний етап у цьому процесі буде видалення доступу веб-бази даних, що використовують як їх основні зберігання даних списків SharePoint.</span><span class="sxs-lookup"><span data-stu-id="0c501-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="0c501-105">Як це впливає на мене?</span><span class="sxs-lookup"><span data-stu-id="0c501-105">How does this affect me?</span></span>

<span data-ttu-id="0c501-106">Починаючи з червня 2019, ми будемо Зупиніть створення нових баз даних Access у SharePoint Online і закриття послуги і всі решта застосунки до 2020 року квітня.</span><span class="sxs-lookup"><span data-stu-id="0c501-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="0c501-107">Що мені потрібно зробити, щоб підготуватися до цієї зміни?</span><span class="sxs-lookup"><span data-stu-id="0c501-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="0c501-108">Ми закликаємо вас створити план переходу для вашої організації веб-доступ до бази даних.</span><span class="sxs-lookup"><span data-stu-id="0c501-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="0c501-109">Адміністратори можна використовувати [застосунок SharePoint доступу сканера](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) для отримання інвентаризація доступ застосунків, які використовують сайти.</span><span class="sxs-lookup"><span data-stu-id="0c501-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="0c501-110">Існує кілька способів перенесення доступ до web баз даних:</span><span class="sxs-lookup"><span data-stu-id="0c501-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="0c501-111">Імпорт локальну базу даних Access (. ACCDB) або файл Excel.</span><span class="sxs-lookup"><span data-stu-id="0c501-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="0c501-112">Ми також рекомендуємо вивчати Microsoft PowerApps як альтернативної платформи для створення бізнесу без коду рішень для веб- і мобільних пристроїв.</span><span class="sxs-lookup"><span data-stu-id="0c501-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>