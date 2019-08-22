---
title: Вміст не відображається в результатах пошуку SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ffb6bf349f9e8c2323186a8fc3183325d1d7e1bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36517052"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="9af0a-102">Вміст не відображається в результатах пошуку SharePoint</span><span class="sxs-lookup"><span data-stu-id="9af0a-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="9af0a-103">Виконайте такі дії під час очікуваних вміст не відображається в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="9af0a-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="9af0a-104">Перевірте, що **сайт** , який містить очікуваного вмісту налаштовані не блокувати вміст з'являтися в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="9af0a-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="9af0a-105">Дотримуйтесь інструкцій у [відображення вмісту сайту в результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="9af0a-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="9af0a-106">Перевірте, що **список** або **бібліотеку** , яка містить очікуваного вмісту налаштовані не блокувати вміст з'являтися в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="9af0a-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="9af0a-107">Дотримуйтесь інструкцій у [відображення вмісту списків або бібліотек в результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="9af0a-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="9af0a-108">Переконайтеся, що сторінки, документ або Розмітка сторінки користувацькі публікуються на **основну версію.**</span><span class="sxs-lookup"><span data-stu-id="9af0a-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="9af0a-109">Виконайте крок 3 в [пошуку не повертає всі результати в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="9af0a-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="9af0a-110">Переконайтеся, що користувач має **права** дозволено переглянути зовнішній вміст.</span><span class="sxs-lookup"><span data-stu-id="9af0a-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="9af0a-111">Виконайте дії у [розумінні рівнів дозволів в SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="9af0a-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="9af0a-112">Якщо пошук схему було змінено, додавши нову керовану властивість, відредагувавши керована властивість або шляхом видалення з керованою властивістю, тоді запит на сканування і повторно проіндексувати вимагатиметься.</span><span class="sxs-lookup"><span data-stu-id="9af0a-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="9af0a-113">**Повторне індексування** вмісту, виконавши дії, зазначені в [Надіслати запит уручну сканування і повторно індексацію сайту, бібліотеку або список](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="9af0a-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="9af0a-114">Це може зайняти деякий час, зачекайте 24 години перед перевіркою результати знову.</span><span class="sxs-lookup"><span data-stu-id="9af0a-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="9af0a-115">Докладніше перегляньте [Увімкнути вміст на сайті, щоб бути придатним для пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="9af0a-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
