---
title: Проблеми, що розвиваються програми з API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975022"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="6624b-102">Проблеми, що розвиваються програми з API</span><span class="sxs-lookup"><span data-stu-id="6624b-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="6624b-103">Щоб почати використовувати API для роботи з програмою Azure Active Directory, ознайомтеся з посібником із короткого посібника з використання служби Azure [AD GRAPH API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , або перегляньте [довідкову документацію API Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="6624b-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="6624b-104">**Кінець підтримки бібліотеки автентифікації в Azure Active Directory (ADAL) та API Azure AD Graph (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="6624b-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="6624b-105">**Починаючи з 30 червня 2020** р., ми більше не додаватимуть нові функції на графіку adal і AZURE AD.</span><span class="sxs-lookup"><span data-stu-id="6624b-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="6624b-106">Ми продовжимо надавати технічну підтримку та оновлення системи безпеки, але більше не зможете надавати оновлення функцій.</span><span class="sxs-lookup"><span data-stu-id="6624b-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="6624b-107">**Починаючи з 30 червня 2022** р., ми ЗАВЕРШУВАТИМЕМО підтримку рекламного графіку Adal і Azure, які більше не зможуть надавати технічну підтримку та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="6624b-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="6624b-108">Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не отримають жодної технічної підтримки або оновлень системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="6624b-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="6624b-109">Програми, що використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки, що відображається в Лазурне AD.</span><span class="sxs-lookup"><span data-stu-id="6624b-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="6624b-110">**Міграція ADAL**</span><span class="sxs-lookup"><span data-stu-id="6624b-110">**ADAL Migration**</span></span>

<span data-ttu-id="6624b-111">Радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="6624b-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="6624b-112">Якщо ви використовуєте програми Microsoft, відомо, що корпорація Майкрософт перебуває в процесі перенесення своїх програм до служби MSAL на термін до кінця підтримки, гарантуючи, що вони будуть користуватися поточною безпекою та удосконаленнями функцій MSAL.</span><span class="sxs-lookup"><span data-stu-id="6624b-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="6624b-113">[Прочитайте запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="6624b-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="6624b-114">[Дізнайтеся, як перенести програми на платформу для кожної платформи](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="6624b-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="6624b-115">Якщо вам потрібна допомога з розумінням, які програми використовують ADAL, радимо переглянути всі вихідні коди програми, а також, якщо це можливо, охопити будь-які постачальники або постачальники програм.</span><span class="sxs-lookup"><span data-stu-id="6624b-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="6624b-116">Служба підтримки Microsoft також може надати вам список всіх програм, які не належать до Microsoft ADAL у вашому клієнті.</span><span class="sxs-lookup"><span data-stu-id="6624b-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="6624b-117">**Міграція AAD графа**</span><span class="sxs-lookup"><span data-stu-id="6624b-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="6624b-118">Для програм, які використовують Azure AD Graph, дотримуйтеся вказівок, щоб перенести [застосунки AZURE AD Graph до Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="6624b-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="6624b-119">[Наш контрольний список перенесення містить точку початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="6624b-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="6624b-120">На порталі реєстрації в програмі Azure App показано, які програми використовують AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="6624b-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="6624b-121">Радимо переглянути всі вихідні коди програм, а також, якщо це можливо, охопити будь-які постачальники ПЗ або провайдери програм.</span><span class="sxs-lookup"><span data-stu-id="6624b-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="6624b-122">Служба підтримки Microsoft також може надати вам список усіх видів використання AAD Graph у вашому клієнті.</span><span class="sxs-lookup"><span data-stu-id="6624b-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="6624b-123">Щоб отримати доступ до даних у програмі Microsoft Graph, користувач або адміністратор має надати йому відповідні дозволи за допомогою процесу згоди.</span><span class="sxs-lookup"><span data-stu-id="6624b-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="6624b-124">[Довідник із дозволів Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) містить список дозволів, пов'язаних із кожним основним набором API Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="6624b-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="6624b-125">Це також дає вказівки про те, як використовувати дозволи.</span><span class="sxs-lookup"><span data-stu-id="6624b-125">It also provides guidance about how to use the permissions.</span></span>
