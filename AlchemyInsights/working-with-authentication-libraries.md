---
title: Робота з бібліотеками автентифікації
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036864"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="6b194-102">Робота з бібліотеками автентифікації</span><span class="sxs-lookup"><span data-stu-id="6b194-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="6b194-103">Щоб вирішити проблему з бібліотекою автентифікації Microsoft (MSAL), виконайте такі Рекомендовані дії:</span><span class="sxs-lookup"><span data-stu-id="6b194-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="6b194-104">**Робота з MSAL**: [бібліотеки автентифікації Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (у цій статті наведено підтримку бібліотеки автентифікації Microsoft для кількох типів програм).</span><span class="sxs-lookup"><span data-stu-id="6b194-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="6b194-105">Вона містить посилання на вихідний код бібліотеки; де можна отримати пакет для проекту програми; і чи підтримує бібліотека підтримку входу (автентифікації) користувача, доступ до захищених веб-API (авторизації) тощо.</span><span class="sxs-lookup"><span data-stu-id="6b194-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="6b194-106">**Виправлення неполадок автентифікації**: msal підтримує кілька потоків автентифікації для використання в різних сценаріях програм.</span><span class="sxs-lookup"><span data-stu-id="6b194-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="6b194-107">Залежно від того, як створюється клієнтська програма, функція MSAL може використовувати один або кілька з потоків автентифікації, які підтримує платформа ідентифікації Microsoft.</span><span class="sxs-lookup"><span data-stu-id="6b194-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="6b194-108">Ці потоки можуть створювати кілька типів маркерів і кодів авторизації, а також вимагати від них різні маркери, щоб вони працювали.</span><span class="sxs-lookup"><span data-stu-id="6b194-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="6b194-109">**Маркери доступу**: [маркери доступу до платформи Microsoft ідентифікації](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) -ДІЗНАЙТЕСЯ, як ваш API може перевіряти та використовувати скарги в маркер доступу.</span><span class="sxs-lookup"><span data-stu-id="6b194-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="6b194-110">Усі документи в цій статті, за винятком випадків, коли вказано, застосовуються лише до маркерів, виданих для API, які ви зареєстрували.</span><span class="sxs-lookup"><span data-stu-id="6b194-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="6b194-111">Він не застосовується до маркерів, виданих для API, які належать до корпорації Майкрософт, і не можуть використовувати маркери, щоб перевірити, як платформа ідентифікації корпорації Майкрософт видає маркери для створеного API.</span><span class="sxs-lookup"><span data-stu-id="6b194-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="6b194-112">**Кінець підтримки бібліотеки автентифікації в Azure Active Directory (ADAL)**</span><span class="sxs-lookup"><span data-stu-id="6b194-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="6b194-113">**Починаючи з 30 червня 2020 р.,** ми більше не додаватимуть нові функції на графіку adal і AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="6b194-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="6b194-114">Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.</span><span class="sxs-lookup"><span data-stu-id="6b194-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="6b194-115">**Починаючи з 30 червня 2022 р.,** ми ЗАВЕРШУВАТИМЕМО підтримку рекламного графіку Adal і Azure, які більше не зможуть надавати технічну підтримку та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="6b194-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="6b194-116">Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не *отримають жодної технічної підтримки або оновлень системи безпеки*.</span><span class="sxs-lookup"><span data-stu-id="6b194-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="6b194-117">Програми, що використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки, що відображається в Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="6b194-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="6b194-118">**Міграція ADAL**</span><span class="sxs-lookup"><span data-stu-id="6b194-118">**ADAL Migration**</span></span>

- <span data-ttu-id="6b194-119">Радимо оновлювати програму MSAL, яка містить найновіші функції та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="6b194-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="6b194-120">Якщо ви використовуєте програми Microsoft, відомо, що корпорація Майкрософт перебуває в процесі перенесення своїх програм до служби MSAL на термін до кінця підтримки, гарантуючи, що вони будуть користуватися поточною безпекою та удосконаленнями функцій MSAL.</span><span class="sxs-lookup"><span data-stu-id="6b194-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="6b194-121">[Прочитайте запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="6b194-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="6b194-122">[Дізнайтеся, як перенести програми на платформу для кожної платформи](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="6b194-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="6b194-123">Якщо після прочитання посібника для платформи програми ви маєте додаткові запитання, ви можете опублікувати [програму Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) за допомогою тега [Azure-AD-adal-nundation] або відкрити проблему в сховищі GitHub в бібліотеці.</span><span class="sxs-lookup"><span data-stu-id="6b194-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="6b194-124">Перегляньте розділ " [мови та структури](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) " в статті " **Огляд msal** " для посилань на службу "РЕПО для кожної бібліотеки".</span><span class="sxs-lookup"><span data-stu-id="6b194-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="6b194-125">**Якщо вам потрібна допомога з розумінням, які програми використовують ADAL**, радимо переглянути всі вихідні коди програм.</span><span class="sxs-lookup"><span data-stu-id="6b194-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="6b194-126">Якщо потрібно, відповідно до будь-яких незалежних постачальників програмного забезпечення (постачальники ISV) або постачальників програм.</span><span class="sxs-lookup"><span data-stu-id="6b194-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="6b194-127">Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому осередку.</span><span class="sxs-lookup"><span data-stu-id="6b194-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







