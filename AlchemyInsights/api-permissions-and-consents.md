---
title: Дозволи для API та згоду
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974998"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="37c06-102">Дозволи для API та згоду</span><span class="sxs-lookup"><span data-stu-id="37c06-102">API permissions and consent</span></span>

<span data-ttu-id="37c06-103">Програми, які інтегруються з ідентифікацією платформи Microsoft, наслідуємо модель авторизації, яка дає користувачам і адміністраторам змогу керувати тим, як можна отримати доступ до даних.</span><span class="sxs-lookup"><span data-stu-id="37c06-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="37c06-104">На кінцевій точці платформи Microsoft ідентифікації оновлено відповідну модель авторизації.</span><span class="sxs-lookup"><span data-stu-id="37c06-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="37c06-105">У цій статті описано, як програма має взаємодіяти з платформою ідентифікації Microsoft.</span><span class="sxs-lookup"><span data-stu-id="37c06-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="37c06-106">[Дозволи та згода в кінцевій точці платформи Microsoft ідентифікації відповідно](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) до основних понять цієї моделі авторизації, зокрема областей, дозволів і згоди.</span><span class="sxs-lookup"><span data-stu-id="37c06-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="37c06-107">[Структура згоди «Лазурний» (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) дає змогу легко розробляти веб-програми з кількома клієнтськими та рідними клієнтами.</span><span class="sxs-lookup"><span data-stu-id="37c06-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="37c06-108">Ці програми дають змогу ввійти за допомогою облікових записів користувачів із Неблакитного РЕКЛАМНОГО клієнта, який відрізняється від того, де буде зареєстрований застосунок.</span><span class="sxs-lookup"><span data-stu-id="37c06-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="37c06-109">Вони також можуть отримати доступ до веб-API, наприклад API Microsoft Graph (щоб отримати доступ до Azure AD, Inune та Services в Microsoft 365) та інших API служб Microsoft Services, крім власного веб-API.</span><span class="sxs-lookup"><span data-stu-id="37c06-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

