---
title: так само, як ім'я файлу краще
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/25/2019
ms.locfileid: "35800066"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="d1c8f-102">Обов'язковий Алхімія заголовок H1, H2's не працюють.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="d1c8f-103">Кращі практики та керівні принципи для алхімії авторська:</span><span class="sxs-lookup"><span data-stu-id="d1c8f-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="d1c8f-104">**Чи не гніздо Алхімія розуміння в папках**-це буде порушувати структуру URL.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="d1c8f-105">Ми дивимося в фіксації цього.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="d1c8f-106">Файли в папці **AlchemyInsights** повинні мати імена нижнього регістру з дефісами для пробілів EX.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="d1c8f-107">***як увімкнути-Судова практика-Hold***.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="d1c8f-108">Додайте ІДЕНТИФІКАТОР правила або код ковша з [порталу Алхімія партнера](https://alchemyportal.azurewebsites.net) в полі MS. Custom.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="d1c8f-109">Колишній.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-109">ex.</span></span> <span data-ttu-id="d1c8f-110">***г. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="d1c8f-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="d1c8f-111">Використайте решту метаданих у верхній частині цього файлу як шаблон.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="d1c8f-112">В [Алхімія партнера порталу](https://alchemyportal.azurewebsites.net), перейдіть до розділу **Insight назва клієнта:** і використовувати це як відправну точку для вашого H1 заголовок для Insight.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="d1c8f-113">Алхімія статистика повинна мати тільки один H1 у верхній або вони будуть ламатися у виробництві.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="d1c8f-114">H2s не відтворювати або використовувати **сміливі** або інші правила для позначення окремих розділів.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="d1c8f-115">Потім заповніть текст тіла за допомогою чернетки матеріалу в розділі "аналітичні огляди клієнтів" на сторінці правила Алхімія</span><span class="sxs-lookup"><span data-stu-id="d1c8f-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="d1c8f-116">Маркіровані списки є штраф</span><span class="sxs-lookup"><span data-stu-id="d1c8f-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="d1c8f-117">Нумеровані списки</span><span class="sxs-lookup"><span data-stu-id="d1c8f-117">Numbered lists too</span></span>
    1. <span data-ttu-id="d1c8f-118">**Жирним шрифтом** і *курсивом* є OK</span><span class="sxs-lookup"><span data-stu-id="d1c8f-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="d1c8f-119">Посилання завжди повинні бути або **"посилання на веб"/зовнішні** або **глибокі посилання на елементи призначеного для користувача інтерфейсу**, а не внутрішні посилання.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="d1c8f-120">Фотографії офіційно не підтримуються в цей час, але це на дорожню карту.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="d1c8f-121">І це дійсно вже трохи занадто довго.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-121">And this is really already a bit too long.</span></span> <span data-ttu-id="d1c8f-122">Краща практика становить близько 400 символів---------------------------------</span><span class="sxs-lookup"><span data-stu-id="d1c8f-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="d1c8f-123">Після того, як ваш контент буде готовий, витягніть його в живу гілку.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="d1c8f-124">Потім перейдіть до [Алхімія партнера порталу](https://alchemyportal.azurewebsites.net) і введіть ім'я файлу в поле URL.</span><span class="sxs-lookup"><span data-stu-id="d1c8f-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 