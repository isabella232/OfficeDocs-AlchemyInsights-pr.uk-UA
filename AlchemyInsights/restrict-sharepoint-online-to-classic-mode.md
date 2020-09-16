---
title: Обмеження служби SharePoint Online на класичний режим
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751444"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="82bba-102">Обмеження служби SharePoint Online на класичний режим</span><span class="sxs-lookup"><span data-stu-id="82bba-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="82bba-103">Деякі організації все ще вимагають класичного режиму роботи.</span><span class="sxs-lookup"><span data-stu-id="82bba-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="82bba-104">Хоча немає планів, щоб видалити класичний режим на гранульованому рівні, не можна обмежувати всю організацію (клієнта) у класичному режимі для списків і бібліотек.</span><span class="sxs-lookup"><span data-stu-id="82bba-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="82bba-105">Адміністратор матиме наведені нижче параметри, щоб керувати окремими списками та бібліотеками в класичному режимі, використовуючи перемикачі гранульовані вимкнення, які ми надаємо на таких рівнях:</span><span class="sxs-lookup"><span data-stu-id="82bba-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="82bba-106">Колекція сайтів</span><span class="sxs-lookup"><span data-stu-id="82bba-106">site collection</span></span>
- <span data-ttu-id="82bba-107">сайт</span><span class="sxs-lookup"><span data-stu-id="82bba-107">site</span></span>
- <span data-ttu-id="82bba-108">списку</span><span class="sxs-lookup"><span data-stu-id="82bba-108">list</span></span>
- <span data-ttu-id="82bba-109">бібліотеки</span><span class="sxs-lookup"><span data-stu-id="82bba-109">library</span></span>

<span data-ttu-id="82bba-110">Крім того, списки, які використовують певні функції та настройки, які не підтримуються в сучасному режимі, все одно буде автоматично змінено на класичний режим.</span><span class="sxs-lookup"><span data-stu-id="82bba-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="82bba-111">Починаючи з 1 квітня 2019, процес вимкнення рівня клієнта вимкнення сучасного списку та бібліотек розпочнеться і продовжиться до 31 травня 2019.</span><span class="sxs-lookup"><span data-stu-id="82bba-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="82bba-112">Списки та бібліотеки, які знаходяться в класичному режимі в результаті вимкнення клієнта, автоматично зсуваються до сучасних.</span><span class="sxs-lookup"><span data-stu-id="82bba-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="82bba-113">Якщо вам потрібен класичний режим, ознайомтеся з додатковими відомостями [тут](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) та інструкцією з PowerShell PnP, що описує варіанти та засоби [, які можна](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) використовувати сьогодні, щоб використовувати класичний режим роботи.</span><span class="sxs-lookup"><span data-stu-id="82bba-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
