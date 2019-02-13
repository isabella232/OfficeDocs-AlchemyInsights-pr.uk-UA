---
title: "так само, як ім'я файлу є кращим [правило #-Опис]"
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 01d8b03209e734f1218de61d964524b1b9e1d044
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29939332"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="7cf61-102">Необхідні Алхімія заголовка H1, H2, не працюють.</span><span class="sxs-lookup"><span data-stu-id="7cf61-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="7cf61-103">Кращі практики і рекомендацій щодо авторинга алхімії:</span><span class="sxs-lookup"><span data-stu-id="7cf61-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="7cf61-p101">**Не гніздяться Алхімія Insights в папках**- це буде ламатися структуру URL-адреси. Ми дивимося на такі виправлення.</span><span class="sxs-lookup"><span data-stu-id="7cf61-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="7cf61-106">Файли в папці **AlchemyInsights** повинна мати правило ID і ім'я правила з [алхімії партнер портал](https://alchemyportal.azurewebsites.net) в імені файлу.</span><span class="sxs-lookup"><span data-stu-id="7cf61-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="7cf61-p102">EX. ***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="7cf61-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="7cf61-p103">Використання метаданих у верхній частині цього файлу як шаблону. Ніщо інше не потрібно.</span><span class="sxs-lookup"><span data-stu-id="7cf61-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="7cf61-111">[Алхімія партнер портал](https://alchemyportal.azurewebsites.net), перейдіть до розділу **замовника Insight заголовок:** і використовувати його як відправна точка для H1 заголовок, за розуміння.</span><span class="sxs-lookup"><span data-stu-id="7cf61-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="7cf61-p104">Алхімія Insights повинні мати тільки одного H1 у верхній частині, або вони буде перерва у виробництві. H2s не візуалізації так використання **жирним** або інші конвенцій, для позначення окремих розділів.</span><span class="sxs-lookup"><span data-stu-id="7cf61-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="7cf61-114">Далі, заповніть основного тексту за допомогою проект матеріалу у розділі клієнтів Insights Алхімія правило сторінки</span><span class="sxs-lookup"><span data-stu-id="7cf61-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="7cf61-115">Маркіровані списки є штраф</span><span class="sxs-lookup"><span data-stu-id="7cf61-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="7cf61-116">Нумеровані списки занадто</span><span class="sxs-lookup"><span data-stu-id="7cf61-116">Numbered lists too</span></span>
    1. <span data-ttu-id="7cf61-117">**Жирний** і *курсив* , a-ok</span><span class="sxs-lookup"><span data-stu-id="7cf61-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="7cf61-118">Посилання повинні бути завжди або **"посилання" / зовнішні** OR **глибокі посилання на елементи Інтерфейсу**, не внутрішні посилання.</span><span class="sxs-lookup"><span data-stu-id="7cf61-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="7cf61-p105">І це дійсно вже трохи занадто довго. Найкраща практика становить близько 400 символів--</span><span class="sxs-lookup"><span data-stu-id="7cf61-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="7cf61-p106">Як тільки ваш контент буде готовий, відповідне вікно виходить жити відділення. Потім перейдіть до [алхімії партнер портал](https://alchemyportal.azurewebsites.net) і введіть ім'я файлу в полі url. Переконайтеся, що Insight переглянуті та опубліковані каже "так" і виберіть правило оновлення. **(Це буде виглядати красивіше, до нової версії порталу - звільнення незабаром).** 
 ![поле url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="7cf61-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

