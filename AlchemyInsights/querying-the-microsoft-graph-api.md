---
title: Запит на створення API Microsoft Graph
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974690"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="d6e40-102">Запит на створення API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="d6e40-103">Цей розділ може також застосовуватися до розробників, які ще використовують API Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="d6e40-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="d6e40-104">Однак **наполегливо** радимо використовувати Microsoft Graph для всіх сценаріїв служби каталогів, посвідчень та керування доступом.</span><span class="sxs-lookup"><span data-stu-id="d6e40-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="d6e40-105">**Проблеми з автентифікацією або авторизацією**</span><span class="sxs-lookup"><span data-stu-id="d6e40-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="d6e40-106">Якщо ваша програма **не може придбати маркери** для виклику Microsoft Graph, виберіть **проблему з використанням маркера доступу (автентифікації)** Microsoft Graph, щоб отримати додаткову довідку й підтримку в цій статті.</span><span class="sxs-lookup"><span data-stu-id="d6e40-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="d6e40-107">Якщо ваша програма **отримує 401 або 403 помилки авторизації** під час виклику Microsoft Graph, виберіть категорію **отримати доступ до помилки (авторизації)** Microsoft Graph API, щоб отримати додаткову довідку й підтримку в цій статті.</span><span class="sxs-lookup"><span data-stu-id="d6e40-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="d6e40-108">**Я хочу використовувати Microsoft Graph, але не знаєте, з чого почати**</span><span class="sxs-lookup"><span data-stu-id="d6e40-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="d6e40-109">Докладні відомості про Microsoft Graph наведено в статті:</span><span class="sxs-lookup"><span data-stu-id="d6e40-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="d6e40-110">Огляд Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="d6e40-111">Огляд ідентифікації та керування доступом у Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="d6e40-112">Початок роботи зі створення програм Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="d6e40-113">**Провідник Microsoft Graph** – перевірка API Microsoft Graph у клієнті або демонстраційному клієнті</span><span class="sxs-lookup"><span data-stu-id="d6e40-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="d6e40-114">**Я хочу використовувати Microsoft Graph, але вона підтримує API 1,0 для каталогу, яку мені потрібно?**</span><span class="sxs-lookup"><span data-stu-id="d6e40-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="d6e40-115">Microsoft Graph – це рекомендований API для каталогів, посвідчень та керування доступом.</span><span class="sxs-lookup"><span data-stu-id="d6e40-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="d6e40-116">Однак, між можливими в лазуровому графіку і Microsoft Graph ще кілька прогалин.</span><span class="sxs-lookup"><span data-stu-id="d6e40-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="d6e40-117">Перегляньте наведені нижче статті, які висвітлюють актуальні відмінності для надання допомоги у виборі:</span><span class="sxs-lookup"><span data-stu-id="d6e40-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="d6e40-118">Відмінності між типами ресурсів у Azure AD Graph і Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="d6e40-119">Відмінності між майновими ОГОЛОШЕННЯМИ та Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="d6e40-120">Відмінності між методами Azure AD і Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="d6e40-121">**Під час запиту на об'єкт *користувача* багато його властивостей відсутні**</span><span class="sxs-lookup"><span data-stu-id="d6e40-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="d6e40-122">`GET https://graph.microsoft.com/v1.0/users` Повертає лише 11 властивостей, оскільки Microsoft Graph автоматично вибирає набір властивостей *користувача* за замовчуванням для повернення.</span><span class="sxs-lookup"><span data-stu-id="d6e40-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="d6e40-123">Якщо вам потрібні інші властивості *користувача* , використовуйте $Select, щоб обрати властивості потреб програми.</span><span class="sxs-lookup"><span data-stu-id="d6e40-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="d6e40-124">Спочатку випробуйте **провідник Microsoft Graph** .</span><span class="sxs-lookup"><span data-stu-id="d6e40-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="d6e40-125">**Деякі значення властивостей користувача мають *Null* -значення, навіть якщо я знаю, що вони налаштовані**</span><span class="sxs-lookup"><span data-stu-id="d6e40-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="d6e40-126">Ймовірніше пояснення полягає в тому, що програма надала *користувачу. ReadBasic. All* дозвіл.</span><span class="sxs-lookup"><span data-stu-id="d6e40-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="d6e40-127">Це дасть змогу програмі читати обмежену кількість властивостей користувача, повернувши всі інші властивості як Null, навіть якщо вони вже були встановлені.</span><span class="sxs-lookup"><span data-stu-id="d6e40-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="d6e40-128">Скористайтеся наданням користувачу застосунку *. читати. Усі* дозволи натомість.</span><span class="sxs-lookup"><span data-stu-id="d6e40-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="d6e40-129">Щоб отримати докладніші відомості, ознайомтеся з [дозволами користувачів Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="d6e40-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="d6e40-130">**У мене виникли проблеми з використанням параметрів запиту OData для фільтрування даних у моїх запитах**</span><span class="sxs-lookup"><span data-stu-id="d6e40-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="d6e40-131">Хоча Microsoft Graph підтримує широкий діапазон параметрів запиту OData, багато з цих параметрів не підтримуються в службах каталогів (ресурси, які успадковуються від *Directoryobject*) у Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d6e40-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="d6e40-132">Ті самі обмеження, які були присутні в лазуровий РЕКЛАМНИЙ графік, зберігаються здебільшого в Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="d6e40-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="d6e40-133">**Не підтримується**: $count, $search та $Filter на *Null* або *не Null* -значення</span><span class="sxs-lookup"><span data-stu-id="d6e40-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="d6e40-134">**Не підтримується**: $Filter за певними властивостями (див. теми ресурсів, у яких властивості можна фільтрувати)</span><span class="sxs-lookup"><span data-stu-id="d6e40-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="d6e40-135">**Не підтримується**: пейджинговий, фільтрація та сортування в той самий час</span><span class="sxs-lookup"><span data-stu-id="d6e40-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="d6e40-136">**Не підтримується**: фільтрування за зв'язком.</span><span class="sxs-lookup"><span data-stu-id="d6e40-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="d6e40-137">Наприклад – знайдіть всіх учасників інженерної групи, що входять до складу Великої Британії.</span><span class="sxs-lookup"><span data-stu-id="d6e40-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="d6e40-138">**Часткова підтримка**: $OrderBy *користувача* (лише Dispиім'я та userPrincipalName) і *Група*</span><span class="sxs-lookup"><span data-stu-id="d6e40-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="d6e40-139">**Часткова підтримка**: $Filter (підтримує тільки " *еквалайзер*", " *startswith*", " *and*", "and" *або* *"обмежена"*), $expand (розширення зв'язків одного об'єкта повертає всі зв'язки, але розширення колекції зв'язків об'єктів обмежена)</span><span class="sxs-lookup"><span data-stu-id="d6e40-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="d6e40-140">Докладні відомості наведено в статті [Настроювання відповідей за допомогою параметрів запиту](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="d6e40-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="d6e40-141">**Виклик API не працює – де можна виконувати додаткові перевірки?**</span><span class="sxs-lookup"><span data-stu-id="d6e40-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="d6e40-142">**Microsoft Graph Explorer** – перевірка API Microsoft Graph у клієнті чи демонстраційному клієнті, а також перегляньте **Приклади запитів** у провіднику Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d6e40-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="d6e40-143">**Під час запиту на дані, схоже, я отримую Неповні дані, які повертаються**</span><span class="sxs-lookup"><span data-stu-id="d6e40-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="d6e40-144">Якщо у вас є запит на збирання (наприклад, *користувачі*), Microsoft Graph використовує серверні обмеження на сторінці, щоб результати завжди були повернуті за замовчуванням розмір сторінки.</span><span class="sxs-lookup"><span data-stu-id="d6e40-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="d6e40-145">Ваша програма має завжди очікувати на сторінку через колекції, повернуті від служби.</span><span class="sxs-lookup"><span data-stu-id="d6e40-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="d6e40-146">Докладні відомості:</span><span class="sxs-lookup"><span data-stu-id="d6e40-146">For more information, see:</span></span>

- [<span data-ttu-id="d6e40-147">Практичні поради з роботи з Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="d6e40-148">Дані про пейджинговий Microsoft Graph у програмі</span><span class="sxs-lookup"><span data-stu-id="d6e40-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="d6e40-149">**Моя програма дуже низька, а також її обмежується. Які удосконалення можна зробити?**</span><span class="sxs-lookup"><span data-stu-id="d6e40-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="d6e40-150">Залежно від сценарію, у вашому розпорядженні є різні варіанти, щоб зробити програму більш продуктивнішою, а в деяких випадках менше схильні до задуми служби (коли ви робите дуже багато розмов).</span><span class="sxs-lookup"><span data-stu-id="d6e40-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="d6e40-151">Докладніше про це див. в статтях:</span><span class="sxs-lookup"><span data-stu-id="d6e40-151">To learn more, see:</span></span>

- [<span data-ttu-id="d6e40-152">Практичні поради з роботи з Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="d6e40-153">Запити на дозування</span><span class="sxs-lookup"><span data-stu-id="d6e40-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="d6e40-154">Відстеження змін через Дельта-запит</span><span class="sxs-lookup"><span data-stu-id="d6e40-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="d6e40-155">Отримання сповіщень про зміни через вебгачки</span><span class="sxs-lookup"><span data-stu-id="d6e40-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="d6e40-156">Вказівки щодо дроселювання</span><span class="sxs-lookup"><span data-stu-id="d6e40-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="d6e40-157">**Де можна знайти додаткові відомості про помилки та відомі проблеми?**</span><span class="sxs-lookup"><span data-stu-id="d6e40-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="d6e40-158">Відомості про помилки під час відгуку Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="d6e40-159">Відомі проблеми з Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="d6e40-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="d6e40-160">**Де можна перевірити стан доступності та підключення служби?**</span><span class="sxs-lookup"><span data-stu-id="d6e40-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="d6e40-161">Доступність служб і зв'язок із базовими службами, які можна отримати за допомогою Microsoft Graph, може вплинути на загальну доступність та продуктивність Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="d6e40-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="d6e40-162">У розділі справність служби "Azure Active Directory" Перевірте стан служби **безпеки + посвідчення** , що відображається на [сторінці "стан Лазур](https://azure.microsoft.com/status/)".</span><span class="sxs-lookup"><span data-stu-id="d6e40-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="d6e40-163">Для служб Office, які беруть участь у програмі Microsoft Graph, перевірте стан служб, перелічених на [приладній дошці служби Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="d6e40-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
