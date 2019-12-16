---
title: Пошук у SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044064"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="f9816-102">Сканування вмісту та індексування в SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f9816-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="f9816-103">Потрібно виконати обхід і додавання вмісту до індексу пошуку, щоб користувачі могли знаходити те, що вони шукають в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f9816-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="f9816-104">Вміст автоматично сканується на основі попередньо визначеного розкладу обходу (розклад обходу не можна змінити).</span><span class="sxs-lookup"><span data-stu-id="f9816-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="f9816-105">Сканер вибирає вміст, який змінився після останнього обходу та оновлює покажчик.</span><span class="sxs-lookup"><span data-stu-id="f9816-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="f9816-106">Щоб забезпечити обхід вмісту та оновлення індексу, зверніть увагу на таке:</span><span class="sxs-lookup"><span data-stu-id="f9816-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="f9816-107">Переконайтеся, що вміст можна знайти, [зробивши вміст сайту доступним для пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="f9816-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="f9816-108">Якщо ви змінили керовану властивість, або коли ви змінили зіставлення обійдених і керованих властивостей, сайт має бути повторно обійдено, перш ніж зміни відобразяться в індексі пошуку.</span><span class="sxs-lookup"><span data-stu-id="f9816-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="f9816-109">Оскільки зміни внесено до схеми пошуку, а не до фактичного сайту, обхідник не буде автоматично повторно індексувати сайт.</span><span class="sxs-lookup"><span data-stu-id="f9816-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="f9816-110">Для отримання додаткових відомостей див [. запит на обхід і повторне індексування сайту, бібліотеки або списку](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="f9816-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="f9816-111">Зачекайте принаймні 24 години після ручного запиту на обхід і повний індекс, щоб дізнатися, чи все ще виникають проблеми.</span><span class="sxs-lookup"><span data-stu-id="f9816-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="f9816-112">Якщо Минуло більше 24 годин, оскільки ви ініціювали обхід і повний індекс, будь ласка, увійдіть у справу підтримки.</span><span class="sxs-lookup"><span data-stu-id="f9816-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="f9816-113">У багатьох випадках ми вже працюємо над вирішенням.</span><span class="sxs-lookup"><span data-stu-id="f9816-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="f9816-114">Будь ласка, дайте нам принаймні 24 годин, щоб завершити рішення.</span><span class="sxs-lookup"><span data-stu-id="f9816-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f9816-115">Якщо сайт, документ (бібліотека) або список було видалено, і все ще відображається в результатах пошуку, користувачі мають отримати **помилку 404 файл не знайдено** під час спроби отримати доступ до нього.</span><span class="sxs-lookup"><span data-stu-id="f9816-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="f9816-116">Ця проблема має реєструватися у випадку підтримки для подальшого розслідування.</span><span class="sxs-lookup"><span data-stu-id="f9816-116">This issue should be logged as a support case for further investigation.</span></span> 



