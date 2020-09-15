---
title: те саме, що й ім'я _ файлу – найкраща
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664155"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="08bb3-102">"Обов'язкове заголовок Алхімія H1, H2's не працює".</span><span class="sxs-lookup"><span data-stu-id="08bb3-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="08bb3-103">Практичні поради та рекомендації з розробки Алхімія:</span><span class="sxs-lookup"><span data-stu-id="08bb3-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="08bb3-104">Не **гніздиться в папках "знання Алхімія**" – це призведе до розриву структури URL-адреси.</span><span class="sxs-lookup"><span data-stu-id="08bb3-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="08bb3-105">Ми шукаємо цю цю інформацію.</span><span class="sxs-lookup"><span data-stu-id="08bb3-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="08bb3-106">Файли в папці **Алліязнання** мають мати малі імена файлів із дефісами для пробілів EX.</span><span class="sxs-lookup"><span data-stu-id="08bb3-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="08bb3-107">***інструкції з включення – судове утримання***.</span><span class="sxs-lookup"><span data-stu-id="08bb3-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="08bb3-108">Включіть код правила або ІДЕНТИФІКАТОР ковша на [порталі партнера Алхімія](https://alchemyportal.azurewebsites.net) в настроюваному полі MS.</span><span class="sxs-lookup"><span data-stu-id="08bb3-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="08bb3-109">Екс.</span><span class="sxs-lookup"><span data-stu-id="08bb3-109">ex.</span></span> <span data-ttu-id="08bb3-110">***MS. Настроювана: 100021***</span><span class="sxs-lookup"><span data-stu-id="08bb3-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="08bb3-111">Використовуйте решту метаданих у верхній частині цього файлу як шаблон.</span><span class="sxs-lookup"><span data-stu-id="08bb3-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="08bb3-112">На [порталі "Алхімія](https://alchemyportal.azurewebsites.net)" перейдіть до розділу " **відомості про назву клієнта** ", а потім використайте його як початкову точку для назви H1 для розуміння.</span><span class="sxs-lookup"><span data-stu-id="08bb3-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="08bb3-113">Знання Алхімія має містити лише один H1 у верхній частині або вони будуть перерватися у виробництві.</span><span class="sxs-lookup"><span data-stu-id="08bb3-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="08bb3-114">У H2s не можна використовувати **жирним шрифтом** або іншими конвенціями для позначення окремих розділів.</span><span class="sxs-lookup"><span data-stu-id="08bb3-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="08bb3-115">Після цього заповніть текст, використовуючи проект "матеріал" в розділі "статистику клієнтів" на сторінці "правило" Алхімія</span><span class="sxs-lookup"><span data-stu-id="08bb3-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="08bb3-116">Маркіровані списки чудово підійдуть</span><span class="sxs-lookup"><span data-stu-id="08bb3-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="08bb3-117">Нумеровані списки</span><span class="sxs-lookup"><span data-stu-id="08bb3-117">Numbered lists too</span></span>
    1. <span data-ttu-id="08bb3-118">**Жирне** та *курсивне накреслення* – це "OK"</span><span class="sxs-lookup"><span data-stu-id="08bb3-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="08bb3-119">Посилання завжди повинні бути як **"посилання на веб"/External** або **глибокими посиланнями на елементи інтерфейсу користувача**, а не внутрішні посилання.</span><span class="sxs-lookup"><span data-stu-id="08bb3-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="08bb3-120">Під час цього часу фотографії офіційно не підтримуються, але це можна робити за допомогою дорожньої карти.</span><span class="sxs-lookup"><span data-stu-id="08bb3-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="08bb3-121">І це вже дуже довгий час.</span><span class="sxs-lookup"><span data-stu-id="08bb3-121">And this is really already a bit too long.</span></span> <span data-ttu-id="08bb3-122">Найкращою практикою є близько 400 символів---------------------------------</span><span class="sxs-lookup"><span data-stu-id="08bb3-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="08bb3-123">Після того як ваш вміст буде готовий, витягніть її в живій гілці.</span><span class="sxs-lookup"><span data-stu-id="08bb3-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="08bb3-124">Потім перейдіть на [портал партнера Алхімія](https://alchemyportal.azurewebsites.net) і введіть ім'я файлу в поле URL-адреса.</span><span class="sxs-lookup"><span data-stu-id="08bb3-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 