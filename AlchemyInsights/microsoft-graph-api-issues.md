---
title: Проблеми з API Microsoft Graph
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
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714518"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="7376a-102">Проблеми з API Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="7376a-103">Цей розділ може також застосовуватися до розробників, які ще використовують API Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="7376a-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="7376a-104">Однак **наполегливо** радимо використовувати Microsoft Graph для всіх сценаріїв служби каталогів, посвідчень та керування доступом.</span><span class="sxs-lookup"><span data-stu-id="7376a-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="7376a-105">**Проблеми з автентифікацією або авторизацією**</span><span class="sxs-lookup"><span data-stu-id="7376a-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="7376a-106">Якщо ваша програма **не може придбати маркери** для виклику Microsoft Graph, виберіть **проблему з використанням маркера доступу (автентифікації)** Microsoft Graph, щоб отримати додаткову довідку й підтримку в цій статті.</span><span class="sxs-lookup"><span data-stu-id="7376a-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="7376a-107">Якщо ваша програма **отримує 401 або 403 помилки авторизації** під час виклику Microsoft Graph, виберіть категорію **отримати доступ до помилки (авторизації)** Microsoft Graph API, щоб отримати додаткову довідку й підтримку в цій статті.</span><span class="sxs-lookup"><span data-stu-id="7376a-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="7376a-108">**Я хочу використовувати Microsoft Graph, але не знаєте, з чого почати**</span><span class="sxs-lookup"><span data-stu-id="7376a-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="7376a-109">Огляд Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="7376a-110">Огляд ідентифікації та керування доступом у Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="7376a-111">Початок роботи зі створення програм Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="7376a-112">**Провідник Microsoft Graph** – перевірка API Microsoft Graph у клієнті або демонстраційному клієнті</span><span class="sxs-lookup"><span data-stu-id="7376a-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="7376a-113">**Я хочу використовувати Microsoft Graph, але вона підтримує API 1,0 для каталогу, яку мені потрібно?**</span><span class="sxs-lookup"><span data-stu-id="7376a-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="7376a-114">Microsoft Graph – це рекомендований API для каталогів, посвідчень та керування доступом.</span><span class="sxs-lookup"><span data-stu-id="7376a-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="7376a-115">Однак, між можливими в лазуровому графіку і Microsoft Graph ще кілька прогалин.</span><span class="sxs-lookup"><span data-stu-id="7376a-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="7376a-116">Перегляньте наведені нижче статті, які висвітлюють актуальні відмінності для надання допомоги у виборі:</span><span class="sxs-lookup"><span data-stu-id="7376a-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="7376a-117">Відмінності між типами ресурсів у Azure AD Graph і Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="7376a-118">Відмінності між майновими ОГОЛОШЕННЯМИ та Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="7376a-119">Відмінності між методами Azure AD і Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="7376a-120">**Під час виклику API не працює – де можна виконувати додаткові перевірки?**</span><span class="sxs-lookup"><span data-stu-id="7376a-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="7376a-121">**Microsoft Graph Explorer** – перевірка API Microsoft Graph у клієнті чи демонстраційному клієнті, а також перегляньте **Приклади запитів** у провіднику Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7376a-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="7376a-122">**Моя програма дуже низька, а також її обмежується. Які удосконалення можна зробити?**</span><span class="sxs-lookup"><span data-stu-id="7376a-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="7376a-123">Залежно від сценарію, у вашому розпорядженні є різні варіанти, щоб зробити програму більш продуктивнішою, а в деяких випадках менше схильні до задуми служби (коли ви робите дуже багато дзвінків).</span><span class="sxs-lookup"><span data-stu-id="7376a-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="7376a-124">Практичні поради з роботи з Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="7376a-125">Запити на дозування</span><span class="sxs-lookup"><span data-stu-id="7376a-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="7376a-126">Відстеження змін через Дельта-запит</span><span class="sxs-lookup"><span data-stu-id="7376a-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="7376a-127">Отримання сповіщень про зміни через вебгачки</span><span class="sxs-lookup"><span data-stu-id="7376a-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="7376a-128">Вказівки щодо дроселювання</span><span class="sxs-lookup"><span data-stu-id="7376a-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="7376a-129">**Де можна знайти додаткові відомості про помилки та відомі проблеми?**</span><span class="sxs-lookup"><span data-stu-id="7376a-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="7376a-130">Відомості про помилки під час відгуку Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="7376a-131">Відомі проблеми з Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="7376a-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="7376a-132">**Де можна перевірити стан доступності та підключення служби?**</span><span class="sxs-lookup"><span data-stu-id="7376a-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="7376a-133">Доступність служб і зв'язок із базовими службами, які можна отримати за допомогою Microsoft Graph, може вплинути на загальну доступність та продуктивність Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7376a-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="7376a-134">У розділі справність служби "Azure Active Directory" Перевірте стан служби **безпеки + посвідчення** , що відображається на [сторінці "стан Лазур](https://azure.microsoft.com/status/)".</span><span class="sxs-lookup"><span data-stu-id="7376a-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="7376a-135">Для служб Office, які беруть участь у програмі Microsoft Graph, перевірте стан служб, перелічених на [приладній дошці служби Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="7376a-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="7376a-136">Помилки авторизації Microsoft Graph можуть бути результатом кількох різних проблем, більшість з яких створює помилку 401 або 403.</span><span class="sxs-lookup"><span data-stu-id="7376a-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="7376a-137">Наприклад, наведені нижче дії можуть призвести до помилок авторизації:</span><span class="sxs-lookup"><span data-stu-id="7376a-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="7376a-138">Неправильні [потоки отримання маркерів доступу](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="7376a-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="7376a-139">Неналежне налаштування [областей дозволів](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="7376a-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="7376a-140">Відсутність [дозволу](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="7376a-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="7376a-141">\**_Кінець підтримки бібліотеки автентифікації Azure Active Directory (ADAL) і API Azure AD Graph (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="7376a-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="7376a-142">_ \* Починаючи з 30 червня 2020 \* \*, ми більше не будемо додавати нові функції до РЕКЛАМНОГО графіку ADAL і Azure.</span><span class="sxs-lookup"><span data-stu-id="7376a-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7376a-143">Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.</span><span class="sxs-lookup"><span data-stu-id="7376a-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="7376a-144">**Починаючи з 30 червня 2022** р., ми ЗАВЕРШУВАТИМЕМО підтримку рекламного графіку Adal і Azure, які більше не зможуть надавати технічну підтримку та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="7376a-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="7376a-145">Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не *отримають жодної технічної підтримки або оновлень системи безпеки*.</span><span class="sxs-lookup"><span data-stu-id="7376a-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="7376a-146">Програми, що використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки, що відображається в Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="7376a-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7376a-147">**Міграція ADAL**</span><span class="sxs-lookup"><span data-stu-id="7376a-147">**ADAL Migration**</span></span>

<span data-ttu-id="7376a-148">Ми радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="7376a-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="7376a-149">Якщо ви використовуєте програми Microsoft, відомо, що корпорація Майкрософт перебуває в процесі перенесення своїх програм до служби MSAL на термін до кінця підтримки, гарантуючи, що вони будуть користуватися поточною безпекою та удосконаленнями функцій MSAL.</span><span class="sxs-lookup"><span data-stu-id="7376a-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="7376a-150">Запитання й відповіді про ADAL</span><span class="sxs-lookup"><span data-stu-id="7376a-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="7376a-151">Дізнайтеся, як перенести програми платформами</span><span class="sxs-lookup"><span data-stu-id="7376a-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="7376a-152">Якщо вам потрібна допомога з розумінням, які програми використовують ADAL, радимо переглянути всі вихідні коди програми, а також, якщо це можливо, охопити будь-які постачальники або постачальники програм.</span><span class="sxs-lookup"><span data-stu-id="7376a-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7376a-153">Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому осередку.</span><span class="sxs-lookup"><span data-stu-id="7376a-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7376a-154">**Перенесення AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="7376a-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="7376a-155">Для програм, які використовують Azure AD Graph, дотримуйтеся вказівок, щоб [перенести застосунки AZURE AD Graph до Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="7376a-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="7376a-156">[Контрольний список перенесення для початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="7376a-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="7376a-157">На порталі реєстрації Azure показано, які програми використовують AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="7376a-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7376a-158">Радимо переглянути вихідний код усіх своїх програм і, за необхідності, зв’язатися з будь-якими незалежними постачальниками програмного забезпечення або постачальниками програм.</span><span class="sxs-lookup"><span data-stu-id="7376a-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7376a-159">Служба підтримки Microsoft також може надати вам список усіх видів використання AAD Graph у вашому клієнті.</span><span class="sxs-lookup"><span data-stu-id="7376a-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="7376a-160">Щоб отримати доступ до даних у програмі Microsoft Graph, користувач або адміністратор має надати йому відповідні дозволи за допомогою процесу згоди.</span><span class="sxs-lookup"><span data-stu-id="7376a-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="7376a-161">[Довідник із дозволів Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) містить список дозволів, пов'язаних із кожним основним набором API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="7376a-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="7376a-162">Це також дає вказівки про те, як використовувати дозволи.</span><span class="sxs-lookup"><span data-stu-id="7376a-162">It also provides guidance about how to use the permissions.</span></span>
