---
title: Проблеми з орендарями
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7824"
- "9004325"
ms.openlocfilehash: 43f75564667bbb952076d4c12d7a1dd1e7e99731
ms.sourcegitcommit: 4e2d640a618c786700e8b276533554d51956f080
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714481"
---
# <a name="issues-with-tenants"></a><span data-ttu-id="3a6c8-102">Проблеми з орендарями</span><span class="sxs-lookup"><span data-stu-id="3a6c8-102">Issues with tenants</span></span>

<span data-ttu-id="3a6c8-103">Azure Active Directory (Azure AD) організовує такі об'єкти, як користувачі та програми в групах, які називаються орендарями.</span><span class="sxs-lookup"><span data-stu-id="3a6c8-103">Azure Active Directory (Azure AD) organizes objects like users and apps into groups called tenants.</span></span> <span data-ttu-id="3a6c8-104">Орендарі дають змогу адміністратору встановлювати політики користувачів в організації, а також про програми, які належить організації, відповідно до їхніх політик безпеки та операційної політики.</span><span class="sxs-lookup"><span data-stu-id="3a6c8-104">Tenants allow an administrator to set policies on the users within the organization and the on apps that the organization owns to meet their security and operational policies.</span></span> <span data-ttu-id="3a6c8-105">Щоб отримати докладніші відомості, ознайомтеся [з оренди в Лазурому Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span><span class="sxs-lookup"><span data-stu-id="3a6c8-105">For more information, see [Tenancy in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/single-and-multi-tenant-apps).</span></span>

<span data-ttu-id="3a6c8-106">Щоб отримати докладніші відомості про керування клієнтом, ознайомтеся з такими статтями:</span><span class="sxs-lookup"><span data-stu-id="3a6c8-106">For more information related to tenant management, see the following articles:</span></span>

- <span data-ttu-id="3a6c8-107">[QuickStart: налаштування](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) клієнта-покаже вам, як створити новий клієнт.</span><span class="sxs-lookup"><span data-stu-id="3a6c8-107">[Quickstart: Set up a tenant](https://docs.microsoft.com/azure/active-directory/develop/quickstart-create-new-tenant) - Shows you how to create a new tenant.</span></span>

- <span data-ttu-id="3a6c8-108">[Видалення клієнта в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) – показує, як видалити клієнта.</span><span class="sxs-lookup"><span data-stu-id="3a6c8-108">[Delete a tenant in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto) - Shows you how to delete a tenant.</span></span>

<span data-ttu-id="3a6c8-109">**Проблеми з кількома орендарями**</span><span class="sxs-lookup"><span data-stu-id="3a6c8-109">**Issues with multi-tenants**</span></span>

<span data-ttu-id="3a6c8-110">Щоб отримати відомості про те, як керувати проблемами, що стосуються кількох орендарів, ознайомтеся з такими статтями:</span><span class="sxs-lookup"><span data-stu-id="3a6c8-110">For information on how to manage issues regarding multi-tenants, see the following articles:</span></span>

- <span data-ttu-id="3a6c8-111">[Як увійти в будь-який користувач Azure Active Directory, використовуючи модель програми для кількох клієнтів,](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) – описано, як перетворити з одного клієнта на багатоклієнтський застосунок.</span><span class="sxs-lookup"><span data-stu-id="3a6c8-111">[How to: Sign in any Azure Active Directory user using the multi-tenant application pattern](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) - Shows you how to convert from a single-tenant to a multi-tenant application.</span></span>
- <span data-ttu-id="3a6c8-112">[Настроювання входу для певної організації «Лазурне Active Directory» в лазуровому Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) – показує, як активувати вхід для користувачів із певної організації «Лазурний», використовуючи потік користувача в ЛАЗУРОВОМУ B2C.</span><span class="sxs-lookup"><span data-stu-id="3a6c8-112">[Set up sign-in for a specific Azure Active Directory organization in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-single-tenant?pivots=b2c-user-flow) - Shows you how to enable sign-in for users from a specific Azure AD organization using a user flow in Azure AD B2C.</span></span>
- <span data-ttu-id="3a6c8-113">[Настроювання входу для багатоклієнтської служби Azure-Active Directory за допомогою спеціальних політик у Лазур Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  вказує, як активувати вхід для користувачів за допомогою кінцевої точки мультиклієнта для служби Azure Active Directory (AZURE AD).</span><span class="sxs-lookup"><span data-stu-id="3a6c8-113">[Set up sign-in for multi-tenant Azure Active Directory using custom policies in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/identity-provider-azure-ad-multi-tenant?pivots=b2c-custom-policy)  shows you how to enable sign-in for users using the multi-tenant endpoint for Azure Active Directory (Azure AD).</span></span>






