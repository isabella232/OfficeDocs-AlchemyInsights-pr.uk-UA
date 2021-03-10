---
title: Пошук сайту
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694553"
---
# <a name="do-site-discovery"></a><span data-ttu-id="396fc-102">Пошук сайту</span><span class="sxs-lookup"><span data-stu-id="396fc-102">Do site discovery</span></span>

<span data-ttu-id="396fc-103">Якщо організація все ще використовує застарілі веб-застосунки та планує використовувати режим Internet Explorer (для більшості клієнтів), потрібно виконати деякі додаткові відкриття сайту.</span><span class="sxs-lookup"><span data-stu-id="396fc-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="396fc-104">**Ви вже розгорнули попередню версію Microsoft EDGE**</span><span class="sxs-lookup"><span data-stu-id="396fc-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="396fc-105">Якщо ви вже налаштували список корпоративних сайтів для роботи в застарілої версії Microsoft EDGE, то відкриття сайту буде майже завершено.</span><span class="sxs-lookup"><span data-stu-id="396fc-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="396fc-106">Можливо, вам потрібно буде додати нейтральні сайти.</span><span class="sxs-lookup"><span data-stu-id="396fc-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="396fc-107">Нейтральні сайти – це зазвичай сайти, які містять єдиний вхід (SSO).</span><span class="sxs-lookup"><span data-stu-id="396fc-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="396fc-108">Якщо ви переходите до нейтрального сайту від Microsoft EDGE, то хочете перебувати в Microsoft EDGE, щоб пройти автентифікацію.</span><span class="sxs-lookup"><span data-stu-id="396fc-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="396fc-109">Якщо ви перейдете на нейтральний сайт у режимі Internet Explorer, ви хочете перебувати в режимі браузера Internet Explorer, щоб автентифікувати.</span><span class="sxs-lookup"><span data-stu-id="396fc-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="396fc-110">Визначте будь-який SSO або інші нейтральні сайти, які ви використовуєте, і додайте їх до списку корпоративних сайтів.</span><span class="sxs-lookup"><span data-stu-id="396fc-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="396fc-111">**Браузер Internet Explorer – це веб-переглядач за замовчуванням**</span><span class="sxs-lookup"><span data-stu-id="396fc-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="396fc-112">Якщо ви зараз використовуєте браузер Internet Explorer, ви можете не знати, які сайти оновлено до сучасних веб-стандартів і що все ще потребують Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="396fc-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="396fc-113">Ви хочете шукати та додавати ці сайти до списку корпоративних сайтів, щоб можна було використовувати режим Internet Explorer лише для цих сайтів.</span><span class="sxs-lookup"><span data-stu-id="396fc-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="396fc-114">[Відкриття корпоративного сайту](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) виявляє сайти, які можуть знадобитися в режимі браузера Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="396fc-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="396fc-115">Вона може збирати дані на комп'ютерах під керуванням Windows Internet Explorer 8 через Internet Explorer 11 в ОС Windows 10, Windows 8,1 або Windows 7.</span><span class="sxs-lookup"><span data-stu-id="396fc-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="396fc-116">**Аналіз даних**</span><span class="sxs-lookup"><span data-stu-id="396fc-116">**Analyze the data**</span></span>

<span data-ttu-id="396fc-117">Після того як ви зібрали дані сайту, ми радимо виконати наведені нижче чотири кроки, щоб аналізувати дані.</span><span class="sxs-lookup"><span data-stu-id="396fc-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="396fc-118">Відсортуйте дані за доменом, а потім за URL-адресою.</span><span class="sxs-lookup"><span data-stu-id="396fc-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="396fc-119">Визначте межі програми, щоб налаштувати режим Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="396fc-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="396fc-120">Потрібно включити всі сайти та веб-елементи керування, які визначають програму, але не потрібно включати додаткові сайти та елементи керування.</span><span class="sxs-lookup"><span data-stu-id="396fc-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="396fc-121">Деякі веб-сайти можуть бути простими, тому що *https://contoso.com/app1* інші можуть вимагати визначення кількох сайтів і сторінок.</span><span class="sxs-lookup"><span data-stu-id="396fc-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="396fc-122">Перевірте програму, щоб переконатися, що вона не працює з самого початку.</span><span class="sxs-lookup"><span data-stu-id="396fc-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="396fc-123">Багато сайтів пропонуватимуть сучасний вміст, коли вони виявляють сучасний браузер і пропонують лише застарілий вміст під час виявлення Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="396fc-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="396fc-124">Додайте програму до списку корпоративних сайтів, якщо це не вдасться виконати тестування.</span><span class="sxs-lookup"><span data-stu-id="396fc-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="396fc-125">Щоб згрупувати всі сайти, які входять до складу програми, рекомендовано.</span><span class="sxs-lookup"><span data-stu-id="396fc-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="396fc-126">Таким чином, під час оновлення програми легше видалити весь сайт із режиму браузера Internet Explorer і почати використовувати сучасний браузер для цієї програми.</span><span class="sxs-lookup"><span data-stu-id="396fc-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="396fc-127">Завершивши Пошук сайтів і ви проаналізували дані, ви готові почати шукати стратегію каналу.</span><span class="sxs-lookup"><span data-stu-id="396fc-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

