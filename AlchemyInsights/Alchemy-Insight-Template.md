---
title: те ж саме ім'я файлу є кращим
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
ms.openlocfilehash: b77e514da36701808d46248e8f2a45137751a1c7
ms.sourcegitcommit: 5447031f9d0a320c49897b8adb5d29ac9437fbc5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/18/2019
ms.locfileid: "35786434"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="c640a-102">Необхідні Алхімія заголовка H1, H2, не працюють.</span><span class="sxs-lookup"><span data-stu-id="c640a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="c640a-103">Кращі практики і рекомендацій щодо авторинга алхімії:</span><span class="sxs-lookup"><span data-stu-id="c640a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="c640a-104">**Не гніздяться Алхімія Insights в папках**- це буде ламатися структуру URL-адреси.</span><span class="sxs-lookup"><span data-stu-id="c640a-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="c640a-105">Ми дивимося на такі виправлення.</span><span class="sxs-lookup"><span data-stu-id="c640a-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="c640a-106">Файли в папці **AlchemyInsights** повинна мати нижній регістр імена файлів на риски для просторів ex.</span><span class="sxs-lookup"><span data-stu-id="c640a-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="c640a-107">***how-to-увімкнути--судового***.</span><span class="sxs-lookup"><span data-stu-id="c640a-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="c640a-108">Включити правило ID або відро ID з [алхімії партнер портал](https://alchemyportal.azurewebsites.net) в ms.custom області.</span><span class="sxs-lookup"><span data-stu-id="c640a-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="c640a-109">EX.</span><span class="sxs-lookup"><span data-stu-id="c640a-109">ex.</span></span> <span data-ttu-id="c640a-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="c640a-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="c640a-111">Використовувати решта метаданих у верхній частині цього файлу як шаблону.</span><span class="sxs-lookup"><span data-stu-id="c640a-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="c640a-112">[Алхімія партнер портал](https://alchemyportal.azurewebsites.net), перейдіть до розділу **замовника Insight заголовок:** і використовувати його як відправна точка для H1 заголовок, за розуміння.</span><span class="sxs-lookup"><span data-stu-id="c640a-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="c640a-113">Алхімія Insights повинні мати тільки одного H1 у верхній частині, або вони буде перерва у виробництві.</span><span class="sxs-lookup"><span data-stu-id="c640a-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="c640a-114">H2s не візуалізації так використання **жирним** або інші конвенцій, для позначення окремих розділів.</span><span class="sxs-lookup"><span data-stu-id="c640a-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="c640a-115">Далі, заповніть основного тексту за допомогою проект матеріалу у розділі клієнтів Insights Алхімія правило сторінки</span><span class="sxs-lookup"><span data-stu-id="c640a-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="c640a-116">Маркіровані списки є штраф</span><span class="sxs-lookup"><span data-stu-id="c640a-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="c640a-117">Нумеровані списки занадто</span><span class="sxs-lookup"><span data-stu-id="c640a-117">Numbered lists too</span></span>
    1. <span data-ttu-id="c640a-118">**Жирний** і *курсив* , a-ok</span><span class="sxs-lookup"><span data-stu-id="c640a-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="c640a-119">Посилання повинні бути завжди або **"посилання" / зовнішні** OR **глибокі посилання на елементи Інтерфейсу**, не внутрішні посилання.</span><span class="sxs-lookup"><span data-stu-id="c640a-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="c640a-120">Фотографії не офіційно підтримуються на даний момент, але це про план дій.</span><span class="sxs-lookup"><span data-stu-id="c640a-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="c640a-121">І це дійсно вже трохи занадто довго.</span><span class="sxs-lookup"><span data-stu-id="c640a-121">And this is really already a bit too long.</span></span> <span data-ttu-id="c640a-122">Найкраща практика становить близько 400 символів--</span><span class="sxs-lookup"><span data-stu-id="c640a-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="c640a-123">Як тільки ваш контент буде готовий, відповідне вікно виходить жити відділення.</span><span class="sxs-lookup"><span data-stu-id="c640a-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="c640a-124">Потім перейдіть до [алхімії партнер портал](https://alchemyportal.azurewebsites.net) і введіть ім'я файлу в полі url.</span><span class="sxs-lookup"><span data-stu-id="c640a-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 


