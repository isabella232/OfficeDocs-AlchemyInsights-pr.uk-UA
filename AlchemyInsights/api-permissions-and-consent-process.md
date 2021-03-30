---
title: Дозволи API та процес згоди
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405445"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="d90be-102">Дозволи API та процес згоди</span><span class="sxs-lookup"><span data-stu-id="d90be-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="d90be-103">Щоб програма отримла доступ до даних у Microsoft Graph, користувач або адміністратор повинен надати їй відповідні дозволи в процесі згоди.</span><span class="sxs-lookup"><span data-stu-id="d90be-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="d90be-104">[Microsoft Graph permissions reference lists](https://docs.microsoft.com/graph/permissions-reference) the permissions associated with each major set of Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="d90be-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="d90be-105">Тут також наведено інструкції з використання дозволів.</span><span class="sxs-lookup"><span data-stu-id="d90be-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="d90be-106">**Настроювання або оновлення основного номера служби**</span><span class="sxs-lookup"><span data-stu-id="d90be-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="d90be-107">[Створення об'єкта-служби. У](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) цій статті описано, як створити об'єкт servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="d90be-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="d90be-108">Створення [основного ім'я](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) служби & Azure AD на порталі. У цій статті описано, як створити нову програму й основне ім'я служби Azure Active Directory (Azure AD), яку можна використовувати з елементом керування доступом на основі ролей.</span><span class="sxs-lookup"><span data-stu-id="d90be-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="d90be-109">[Принципи програм &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) служби в Azure AD. У цій статті описано реєстрацію програм, об'єкти програм і основні імена служб в Azure Active Directory: їхнє призначення, а також те, як вони пов'язані між собою.</span><span class="sxs-lookup"><span data-stu-id="d90be-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="d90be-110">**Додавання або оновлення реєстрації програм і надання згоди адміністратора**</span><span class="sxs-lookup"><span data-stu-id="d90be-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="d90be-111">[Створіть реєстрацію програми.](https://docs.microsoft.com/graph/api/application-post-applications) У цій статті описано, як створити об'єкт програми.</span><span class="sxs-lookup"><span data-stu-id="d90be-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="d90be-112">[Оновлення реєстрації програми – дозволи API.](https://docs.microsoft.com/graph/api/application-update) У цій статті описано, як оновити властивості об'єкта програми.</span><span class="sxs-lookup"><span data-stu-id="d90be-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="d90be-113">[Надайте згоду](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) адміністратора. Щоб отримати згоду адміністратора та надати згоду в цілому, адміністратор має явно надати згоду.</span><span class="sxs-lookup"><span data-stu-id="d90be-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="d90be-114">[RBAC (бета-система).](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) Контейнер керування ролями для уніфікованих визначень ролей і призначень ролей для постачальників Microsoft 365 RBAC, який підтримує кілька основних ролей і кількох областей в одному призначенні ролей.</span><span class="sxs-lookup"><span data-stu-id="d90be-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="d90be-115">Цей тип ресурсу *відрізняється від типу ресурсу rbacApplication.*</span><span class="sxs-lookup"><span data-stu-id="d90be-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="d90be-116">Microsoft Intune – приклад такого постачальника RBAC.</span><span class="sxs-lookup"><span data-stu-id="d90be-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="d90be-117">Призначення ролей в Intune може мати масив основних значень і масив груп областей.</span><span class="sxs-lookup"><span data-stu-id="d90be-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="d90be-118">**Це в бета-програмі, тобто вона ще на стадіях розробки та не рекомендується для використання в виробництво.**</span><span class="sxs-lookup"><span data-stu-id="d90be-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
