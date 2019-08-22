---
title: Керувати пошук схеми в SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 704fb3b682d23220d61192e383d7d80f59f27933
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502828"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="ea887-102">Керувати пошук схеми в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="ea887-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="ea887-103">Пошук схеми контролює те, що користувачі можуть шукати, як користувачі можуть шукати його, і як можна демонструвати результати пошуку веб-сайтів.</span><span class="sxs-lookup"><span data-stu-id="ea887-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="ea887-104">Див. [керування SharePoint Online, схеми пошук](https://docs.microsoft.com/sharepoint/manage-search-schema) щоб дізнатися як:</span><span class="sxs-lookup"><span data-stu-id="ea887-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="ea887-105">Змінити схему пошуку.</span><span class="sxs-lookup"><span data-stu-id="ea887-105">Change the search schema.</span></span>
- <span data-ttu-id="ea887-106">Створення керованих властивостей.</span><span class="sxs-lookup"><span data-stu-id="ea887-106">Create managed properties.</span></span>
- <span data-ttu-id="ea887-107">Властивості виконаного обходу карту обійденого карту з керованими властивостями.</span><span class="sxs-lookup"><span data-stu-id="ea887-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="ea887-108">Пам'ятайте про таке відносно керування пошук схеми:</span><span class="sxs-lookup"><span data-stu-id="ea887-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="ea887-109">Якщо ви отримуєте попередження, заявивши, що **застосування призупинено** коли внесення змін схеми, це лише тимчасові як сервісне обслуговування, що відбуваються.</span><span class="sxs-lookup"><span data-stu-id="ea887-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="ea887-110">Якщо Минуло більше, ніж за 24 години, і ви все ще відчувають попередження, будь ласка, увійдіть інциденту до служби підтримки.</span><span class="sxs-lookup"><span data-stu-id="ea887-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="ea887-111">Під час змінення керованих властивостей або додати нові, зміни набудуть чинності лише після того, як вміст було повторно виконаного обходу.</span><span class="sxs-lookup"><span data-stu-id="ea887-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="ea887-112">У SharePoint Online сканування відбувається автоматично на основі визначених обходу графіком.</span><span class="sxs-lookup"><span data-stu-id="ea887-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="ea887-113">Щоб переконатися, що сканується зміни, ви можете спеціально [переіндексація списку або бібліотеки прохання](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="ea887-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="ea887-114">Повний огляд пошук схеми див [Введення пошуку схеми](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="ea887-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


