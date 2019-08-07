---
title: Пошук у SharePoint онлайн
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059273"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="f42db-102">Пошук у SharePoint онлайн</span><span class="sxs-lookup"><span data-stu-id="f42db-102">Search in SharePoint Online</span></span>

<span data-ttu-id="f42db-103">Зміст повинен бути поповз і додано до індексу пошуку для користувачів, щоб знайти те, що вони шукають у SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f42db-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="f42db-104">Вміст виконується обхід автоматично на основі попередньо визначеного обходу розкладом (розклад обходу змінити не можна).</span><span class="sxs-lookup"><span data-stu-id="f42db-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="f42db-105">Обхіднику підбирає вміст, який змінився з моменту здійснення останнього обходу та оновлює індексу.</span><span class="sxs-lookup"><span data-stu-id="f42db-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="f42db-106">Щоб переконатися, що виконується обхід вмісту та оновлення індексу, зверніть увагу на таке:</span><span class="sxs-lookup"><span data-stu-id="f42db-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="f42db-107">Переконайтеся, що вміст може бути знайдений шляхом [прийняття вмісту сайту для пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="f42db-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="f42db-108">Коли ви змінили керовану властивість, або коли ви змінили зіставлення, поповз і вдалося властивості, сайт має бути повторно обійденого перш ніж внесені зміни буде застосовано до індексу пошуку.</span><span class="sxs-lookup"><span data-stu-id="f42db-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="f42db-109">Тому що ваш вносяться зміни у схемі пошуку а не власне на сайт, обхідник не автоматично повторно індексуватимемо сайту.</span><span class="sxs-lookup"><span data-stu-id="f42db-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="f42db-110">Для отримання додаткових відомостей див. [Надіслати запит уручну сканування і повторно індексацію сайту, бібліотеку або список](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="f42db-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="f42db-111">Зачекайте принаймні 24 години після вручну запитуючої сканування і повне повторне індексування бачити, якщо ви все ще відчувають проблеми.</span><span class="sxs-lookup"><span data-stu-id="f42db-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="f42db-112">Якщо з вам ініційований обходу і повний буде повторно проіндексувати Минуло більше 24 годин, будь ласка, увійдіть інциденту до служби підтримки.</span><span class="sxs-lookup"><span data-stu-id="f42db-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="f42db-113">У багатьох випадках ми вже працюємо над вирішенням.</span><span class="sxs-lookup"><span data-stu-id="f42db-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f42db-114">Будь ласка, надайте нам принаймні за 24 години до виконання рішення.</span><span class="sxs-lookup"><span data-stu-id="f42db-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Зверніть увагу!]<span data-ttu-id="f42db-115">: якщо сайт, документ (бібліотека) або список був видалений і до цих пір шоу в результатах пошуку, користувачі повинні отримувати **Помилка 404 файлів не знайшли** при спробі доступу до нього.</span><span class="sxs-lookup"><span data-stu-id="f42db-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="f42db-116">Це питання повинен реєструватися як інциденту до служби підтримки для подальшого розслідування.</span><span class="sxs-lookup"><span data-stu-id="f42db-116">This issue should be logged as a support case for further investigation.</span></span> 



