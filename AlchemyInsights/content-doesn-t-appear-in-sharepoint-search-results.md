---
title: Вміст не відображається в результатах пошуку в службі SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713151"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="0e715-102">Вміст не відображається в результатах пошуку в службі SharePoint</span><span class="sxs-lookup"><span data-stu-id="0e715-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="0e715-103">Виконайте ці кроки з виправлення неполадок, коли очікуваний вміст не відображається в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="0e715-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="0e715-104">Переконайтеся, що для **сайту** , який містить очікуваний вміст, установіть прапорець Дозволити вміст відображатися в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="0e715-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0e715-105">Виконайте вказівки, описані в розділі [відображення вмісту на сайті в результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0e715-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="0e715-106">Переконайтеся, що для **списку** або **бібліотеки** , яка містить очікуваний вміст, установіть прапорець Дозволити вміст відображатися в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="0e715-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="0e715-107">Виконайте вказівки, описані в розділі [відображення вмісту зі списків або бібліотек у результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="0e715-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="0e715-108">Переконайтеся, що для сторінки, документа або настроюваного макета сторінки Опубліковано як **Основна версія.**</span><span class="sxs-lookup"><span data-stu-id="0e715-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="0e715-109">Виконайте крок 3 в [результатах пошуку, не повертають всі результати в службі SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="0e715-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="0e715-110">Переконайтеся, що користувач має **дозволи** на перегляд вмісту.</span><span class="sxs-lookup"><span data-stu-id="0e715-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="0e715-111">Виконайте вказівки, описані в статті [Загальні відомості про рівні дозволів у службі SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="0e715-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="0e715-112">Якщо схему пошуку змінено, додавши нову керовану властивість, редагуючи керовану властивість, або видаливши керовану властивість, а потім потрібно буде виконати запит на обхід та повторно індексувати.</span><span class="sxs-lookup"><span data-stu-id="0e715-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="0e715-113">**Повторно індексувати** вміст, виконавши вказівки, описані в [запиті вручну обхід та повторне індексування сайту, бібліотеки або списку](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="0e715-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="0e715-114">Це може тривати деякий час, зачекайте 24 години, перш ніж знову перевірити результати.</span><span class="sxs-lookup"><span data-stu-id="0e715-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="0e715-115">Докладні відомості наведено в статті [Увімкнення вмісту сайту для пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="0e715-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
