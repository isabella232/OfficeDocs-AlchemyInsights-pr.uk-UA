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
ms.openlocfilehash: e248c2ee3cbb9a86f21c1f36be10c893df76ff52
ms.sourcegitcommit: 3070905131e6d8449981231a3551c0bb4ca38ae6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/14/2019
ms.locfileid: "30634525"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="c885d-102">Необхідні Алхімія заголовка H1, H2, не працюють.</span><span class="sxs-lookup"><span data-stu-id="c885d-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="c885d-103">Кращі практики і рекомендацій щодо авторинга алхімії:</span><span class="sxs-lookup"><span data-stu-id="c885d-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="c885d-104">**Не гніздяться Алхімія Insights в папках**- це буде ламатися структуру URL-адреси.</span><span class="sxs-lookup"><span data-stu-id="c885d-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="c885d-105">Ми дивимося на такі виправлення.</span><span class="sxs-lookup"><span data-stu-id="c885d-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="c885d-106">Файли в папці **AlchemyInsights** повинна мати правило ID і ім'я правила з [алхімії партнер портал](https://alchemyportal.azurewebsites.net) в імені файлу.</span><span class="sxs-lookup"><span data-stu-id="c885d-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="c885d-107">EX.</span><span class="sxs-lookup"><span data-stu-id="c885d-107">ex.</span></span> <span data-ttu-id="c885d-108">***976-How-To-Enable-Litigation-Hold***</span><span class="sxs-lookup"><span data-stu-id="c885d-108">***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="c885d-109">Використання метаданих у верхній частині цього файлу як шаблону.</span><span class="sxs-lookup"><span data-stu-id="c885d-109">Use the metadata at the top of this file as your template.</span></span> <span data-ttu-id="c885d-110">Ніщо інше не потрібно.</span><span class="sxs-lookup"><span data-stu-id="c885d-110">Nothing else is required.</span></span>
1. <span data-ttu-id="c885d-111">[Алхімія партнер портал](https://alchemyportal.azurewebsites.net), перейдіть до розділу **замовника Insight заголовок:** і використовувати його як відправна точка для H1 заголовок, за розуміння.</span><span class="sxs-lookup"><span data-stu-id="c885d-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="c885d-112">Алхімія Insights повинні мати тільки одного H1 у верхній частині, або вони буде перерва у виробництві.</span><span class="sxs-lookup"><span data-stu-id="c885d-112">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="c885d-113">H2s не візуалізації так використання **жирним** або інші конвенцій, для позначення окремих розділів.</span><span class="sxs-lookup"><span data-stu-id="c885d-113">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="c885d-114">Далі, заповніть основного тексту за допомогою проект матеріалу у розділі клієнтів Insights Алхімія правило сторінки</span><span class="sxs-lookup"><span data-stu-id="c885d-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="c885d-115">Маркіровані списки є штраф</span><span class="sxs-lookup"><span data-stu-id="c885d-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="c885d-116">Нумеровані списки занадто</span><span class="sxs-lookup"><span data-stu-id="c885d-116">Numbered lists too</span></span>
    1. <span data-ttu-id="c885d-117">**Жирний** і *курсив* , a-ok</span><span class="sxs-lookup"><span data-stu-id="c885d-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="c885d-118">Посилання повинні бути завжди або **"посилання" / зовнішні** OR **глибокі посилання на елементи Інтерфейсу**, не внутрішні посилання.</span><span class="sxs-lookup"><span data-stu-id="c885d-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="c885d-119">І це дійсно вже трохи занадто довго.</span><span class="sxs-lookup"><span data-stu-id="c885d-119">And this is really already a bit too long.</span></span> <span data-ttu-id="c885d-120">Найкраща практика становить близько 400 символів--</span><span class="sxs-lookup"><span data-stu-id="c885d-120">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="c885d-121">Як тільки ваш контент буде готовий, відповідне вікно виходить жити відділення.</span><span class="sxs-lookup"><span data-stu-id="c885d-121">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="c885d-122">Потім перейдіть до [алхімії партнер портал](https://alchemyportal.azurewebsites.net) і введіть ім'я файлу в полі url.</span><span class="sxs-lookup"><span data-stu-id="c885d-122">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="c885d-123">Переконайтеся, що Insight переглянуті та опубліковані каже "так" і виберіть правило оновлення.</span><span class="sxs-lookup"><span data-stu-id="c885d-123">Make sure Insight reviewed and published says "yes" and then click Update Rule.</span></span> <span data-ttu-id="c885d-124">**(Це буде виглядала до нової версії порталу - незабаром випускати.)** 
 ![поле url](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="c885d-124">**(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

