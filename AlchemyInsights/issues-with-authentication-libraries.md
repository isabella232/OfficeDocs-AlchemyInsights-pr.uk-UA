---
title: Проблеми з бібліотеками автентифікації
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063703"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="5a38f-102">Проблеми з бібліотеками автентифікації</span><span class="sxs-lookup"><span data-stu-id="5a38f-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="5a38f-103">[Бібліотеки автентифікації в програмі Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) , що підтримуються, і сумісні з ними, а бібліотеки з підтримкою Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5a38f-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="5a38f-104">Бібліотека автентифікації Microsoft (MSAL) підтримує кілька [потоків автентифікації](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) для використання в різних сценаріях програм.</span><span class="sxs-lookup"><span data-stu-id="5a38f-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="5a38f-105">Щоб автентифікувати та придбати маркери, ви ініціалізаєте нову загальнодоступну або конфіденційну клієнтську програму в коді.</span><span class="sxs-lookup"><span data-stu-id="5a38f-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="5a38f-106">Під час ініціалізації програми клієнта в бібліотеці автентифікації Microsoft (MSAL) можна настроїти кілька параметрів конфігурації.</span><span class="sxs-lookup"><span data-stu-id="5a38f-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="5a38f-107">Докладні відомості наведено в статті [Параметри конфігурації застосунку](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="5a38f-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="5a38f-108">**Кінець підтримки бібліотеки автентифікації в Azure Active Directory (ADAL) та API Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="5a38f-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="5a38f-109">**Починаючи з 30 червня 2020** р., ми більше не додаватимуть нові функції на графіку adal і AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="5a38f-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="5a38f-110">Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.</span><span class="sxs-lookup"><span data-stu-id="5a38f-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="5a38f-111">**Починаючи з 30 червня 2022** р., ми ЗАВЕРШУВАТИМЕМО підтримку рекламного графіку Adal і Azure, які більше не зможуть надавати технічну підтримку та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="5a38f-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="5a38f-112">Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не *отримають жодної технічної підтримки або оновлень системи безпеки*.</span><span class="sxs-lookup"><span data-stu-id="5a38f-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="5a38f-113">Програми, що використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки, що відображається в Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="5a38f-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="5a38f-114">**Міграція ADAL**</span><span class="sxs-lookup"><span data-stu-id="5a38f-114">**ADAL Migration**</span></span>

<span data-ttu-id="5a38f-115">Ми радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="5a38f-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="5a38f-116">Якщо ви використовуєте програми Microsoft, відомо, що корпорація Майкрософт перебуває в процесі перенесення своїх програм до служби MSAL на термін до кінця підтримки, гарантуючи, що вони отримають вигоду від поточної системи безпеки й вдосконалення функцій MSAL.</span><span class="sxs-lookup"><span data-stu-id="5a38f-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="5a38f-117">Докладні відомості:</span><span class="sxs-lookup"><span data-stu-id="5a38f-117">For more information, see:</span></span>

1. [<span data-ttu-id="5a38f-118">Запитання й відповіді про ADAL</span><span class="sxs-lookup"><span data-stu-id="5a38f-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="5a38f-119">Дізнайтеся, як перенести програми платформами</span><span class="sxs-lookup"><span data-stu-id="5a38f-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="5a38f-120">Якщо вам потрібна допомога з розумінням, які програми використовують ADAL, радимо переглянути всі вихідні коди програми, а також, якщо це можливо, охопити будь-які постачальники або постачальники програм.</span><span class="sxs-lookup"><span data-stu-id="5a38f-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="5a38f-121">Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому клієнті.</span><span class="sxs-lookup"><span data-stu-id="5a38f-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="5a38f-122">**Перенесення AAD Graph**</span><span class="sxs-lookup"><span data-stu-id="5a38f-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="5a38f-123">Для програм, які використовують Azure AD Graph, дотримуйтеся вказівок, щоб [перенести застосунки AZURE AD Graph до Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="5a38f-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="5a38f-124">Наш контрольний список перенесення містить точку початку роботи.</span><span class="sxs-lookup"><span data-stu-id="5a38f-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="5a38f-125">На порталі реєстрації Azure показано, які програми використовують AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="5a38f-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="5a38f-126">Радимо переглянути вихідний код усіх своїх програм і, за необхідності, зв’язатися з будь-якими незалежними постачальниками програмного забезпечення або постачальниками програм.</span><span class="sxs-lookup"><span data-stu-id="5a38f-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="5a38f-127">Служба підтримки Microsoft також може надати вам список усіх видів використання AAD Graph у вашому клієнті.</span><span class="sxs-lookup"><span data-stu-id="5a38f-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="5a38f-128">Щоб отримати доступ до даних у програмі Microsoft Graph, користувач або адміністратор має надати йому відповідні дозволи за допомогою процесу згоди.</span><span class="sxs-lookup"><span data-stu-id="5a38f-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="5a38f-129">[Довідник із дозволів Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) містить список дозволів, пов'язаних із кожним основним набором API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="5a38f-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="5a38f-130">Це також дає вказівки про те, як використовувати дозволи.</span><span class="sxs-lookup"><span data-stu-id="5a38f-130">It also provides guidance about how to use the permissions.</span></span>
