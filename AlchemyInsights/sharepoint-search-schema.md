---
title: Керування схемою пошуку в службі SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770572"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="bb5cd-102">Керування схемою пошуку в службі SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="bb5cd-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="bb5cd-103">Схема пошуку керує тим, що користувачі можуть шукати, як користувачі можуть шукати його, а також про те, як можна представити результати на веб-сайтах пошуку.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="bb5cd-104">Дізнайтеся [, як керувати схемою пошуку в службі SharePoint Online,](https://docs.microsoft.com/sharepoint/manage-search-schema) щоб дізнатися, як це зробити:</span><span class="sxs-lookup"><span data-stu-id="bb5cd-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="bb5cd-105">Змінення схеми пошуку.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-105">Change the search schema.</span></span>
- <span data-ttu-id="bb5cd-106">Створення керованих властивостей.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-106">Create managed properties.</span></span>
- <span data-ttu-id="bb5cd-107">Зіставте карту обійденого елемента, у якій можна керувати керованими властивостями.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="bb5cd-108">Зверніть увагу на те, як керувати схемою пошуку, виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="bb5cd-109">Якщо ви отримали попередження про те, **що програма призупиняється** під час внесення змін до схеми, це тимчасовий характер, оскільки відбувається обслуговування служби.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="bb5cd-110">Якщо Минуло більше 24 годин, і ви все ще відчуєте попередження, увійдіть у справу підтримки.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="bb5cd-111">Якщо змінити керовані властивості або додати нові, зміни набули чинності лише після повторного обходу вмісту.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="bb5cd-112">У службі SharePoint Online обхід відбувається автоматично на основі визначеного розкладу обходу.</span><span class="sxs-lookup"><span data-stu-id="bb5cd-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="bb5cd-113">Щоб переконатися, що зміни обійдено, можна конкретно [Надіслати запит на переіндексування списку або бібліотеки](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list) .</span><span class="sxs-lookup"><span data-stu-id="bb5cd-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="bb5cd-114">Повний огляд схеми пошуку наведено в статті Загальні відомості про [схему](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/) пошуку</span><span class="sxs-lookup"><span data-stu-id="bb5cd-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


