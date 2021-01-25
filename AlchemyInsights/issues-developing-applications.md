---
title: Проблеми з розробкою програм
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974763"
---
# <a name="issues-developing-applications"></a><span data-ttu-id="42afa-102">Проблеми з розробкою програм</span><span class="sxs-lookup"><span data-stu-id="42afa-102">Issues developing applications</span></span>

<span data-ttu-id="42afa-103">Щоб усунути найпоширеніші проблеми під час створення веб-програм "блакитні активні каталоги (AD)", ознайомтеся з такими статтями:</span><span class="sxs-lookup"><span data-stu-id="42afa-103">To troubleshoot the most common problems when building Azure Active Directory (AD) apps, see the following articles:</span></span>

- [<span data-ttu-id="42afa-104">Я бачу проблеми з входом в програму лише за допомогою браузера Chrome</span><span class="sxs-lookup"><span data-stu-id="42afa-104">I am seeing trouble signing in to application(s) using Chrome browser only</span></span>](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [<span data-ttu-id="42afa-105">Я не знаю, як змінити параметри терміну дії маркера для моєї програми</span><span class="sxs-lookup"><span data-stu-id="42afa-105">I don't know how to change the token lifetime defaults for my application</span></span>](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [<span data-ttu-id="42afa-106">Я заплутався про те, як працює згода на використання програми</span><span class="sxs-lookup"><span data-stu-id="42afa-106">I am confused about how application consent works</span></span>](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [<span data-ttu-id="42afa-107">Я не знаю, як надати дозволи для моєї програми</span><span class="sxs-lookup"><span data-stu-id="42afa-107">I don't know how to grant permissions to my application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [<span data-ttu-id="42afa-108">Я не можу розібратися в різниці між делегованих і дозволами на використання програми</span><span class="sxs-lookup"><span data-stu-id="42afa-108">I don't understand the difference between delegated and application permissions</span></span>](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

<span data-ttu-id="42afa-109">\***Кінець підтримки бібліотеки автентифікації в Azure Active Directory (ADAL) та API AZURE AD Graph (AAD Graph)** _</span><span class="sxs-lookup"><span data-stu-id="42afa-109">\***End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)** _</span></span>

- <span data-ttu-id="42afa-110">Починаючи з 30 червня 2020, ми більше не додаватимуть нові функції в бібліотеці автентифікації Azure Active Directory (ADAL) і Azure AD Graph API (AAD Graph).</span><span class="sxs-lookup"><span data-stu-id="42afa-110">Starting June 30th, 2020, we will no longer add any new features to Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph).</span></span> <span data-ttu-id="42afa-111">Ми продовжимо надавати технічну підтримку та оновлення системи безпеки, але більше не зможете надавати оновлення функцій.</span><span class="sxs-lookup"><span data-stu-id="42afa-111">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

- <span data-ttu-id="42afa-112">Починаючи з 30 червня 2022 р., ми завершуємо підтримку на графіку ADAL і AAD, і більше не зможете надавати технічну підтримку та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="42afa-112">Starting June 30th, 2022, we will end support for ADAL and AAD Graph and will no longer provide technical support or security updates.</span></span> <span data-ttu-id="42afa-113">У результаті цієї умови наведені нижче наслідки наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="42afa-113">As a result of this condition, the following are the implications:</span></span>

    - <span data-ttu-id="42afa-114">Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не отримають жодної технічної підтримки або оновлень системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="42afa-114">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

    - <span data-ttu-id="42afa-115">Програми, що використовують AAD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки AAD графа</span><span class="sxs-lookup"><span data-stu-id="42afa-115">Apps using AAD Graph after this time may no longer receive responses from the AAD Graph endpoint</span></span>

<span data-ttu-id="42afa-116">_ *Adal перенесення*\*</span><span class="sxs-lookup"><span data-stu-id="42afa-116">_ *ADAL Migration*\*</span></span>

<span data-ttu-id="42afa-117">Якщо ви використовуєте програми Microsoft, радимо оновити бібліотеку автентифікації Microsoft (MSAL), яка містить найновіші функції та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="42afa-117">If you're using Microsoft apps, we recommend updating to the Microsoft Authentication Library (MSAL), which has the latest features and security updates.</span></span> <span data-ttu-id="42afa-118">Ця рекомендація в контексті Microsoft ініціює процес перенесення своїх програм до MSAL до кінцевого терміну підтримки.</span><span class="sxs-lookup"><span data-stu-id="42afa-118">This recommendation is in the context of Microsoft initiating the process of migrating its apps to MSAL by the end-of-support deadline.</span></span> 

<span data-ttu-id="42afa-119">Міграція корпорацією Майкрософт своїх програм для MSAL гарантує, що програми отримують вигоду від поточної безпеки та удосконалень функцій MSAL.</span><span class="sxs-lookup"><span data-stu-id="42afa-119">The migration by Microsoft of its apps to MSAL ensures that the apps benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="42afa-120">Читайте запитання й відповіді про ADAL</span><span class="sxs-lookup"><span data-stu-id="42afa-120">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [<span data-ttu-id="42afa-121">Відомості про перенесення програм на основі платформи</span><span class="sxs-lookup"><span data-stu-id="42afa-121">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. <span data-ttu-id="42afa-122">Якщо вам потрібна допомога в розумінні того, що ваші програми використовують ADAL, радимо переглянути всі вихідні коди програм і, за потреби, відповідати всім незалежним постачальникам програмного забезпечення (постачальникам ПЗ) або постачальникам програм.</span><span class="sxs-lookup"><span data-stu-id="42afa-122">If you need help in understanding which of your apps use ADAL, we recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="42afa-123">Служба підтримки Microsoft також може надати вам список всіх програм, які не належать до Microsoft ADAL у вашому клієнті.</span><span class="sxs-lookup"><span data-stu-id="42afa-123">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="42afa-124">**Міграція AAD графа**</span><span class="sxs-lookup"><span data-stu-id="42afa-124">**AAD Graph Migration**</span></span>

<span data-ttu-id="42afa-125">Для програм, що використовують AAD Graph, дотримуйтеся вказівок, щоб перенести програми AAD Graph до Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="42afa-125">For applications that are using AAD Graph, follow our guidance to migrate AAD Graph apps to Microsoft Graph:</span></span>

1. <span data-ttu-id="42afa-126">[Наш контрольний список перенесення містить точку початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="42afa-126">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
2. <span data-ttu-id="42afa-127">На порталі реєстрації в програмі Azure App показано, які програми використовують AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="42afa-127">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="42afa-128">Радимо переглянути всі вихідні коди програм і, за необхідності, охопити будь-які незалежні постачальники програмного забезпечення (незалежні постачальники ПЗ) або постачальники програм.</span><span class="sxs-lookup"><span data-stu-id="42afa-128">We recommend you review all of your apps' source code and, if applicable, reach out to any independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="42afa-129">Служба підтримки Microsoft також може надати вам інформацію про використання графіків у вашому клієнті.</span><span class="sxs-lookup"><span data-stu-id="42afa-129">Microsoft support can also provide you information on AAD Graph usage in your tenant.</span></span>







