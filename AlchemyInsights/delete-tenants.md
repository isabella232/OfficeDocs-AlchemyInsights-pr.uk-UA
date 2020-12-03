---
title: Видалення клієнта
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564876"
---
# <a name="delete-tenant"></a><span data-ttu-id="7311a-102">Видалення клієнта</span><span class="sxs-lookup"><span data-stu-id="7311a-102">Delete tenant</span></span>

<span data-ttu-id="7311a-103">Щоб видалити Azure AD, переконайтеся, що:</span><span class="sxs-lookup"><span data-stu-id="7311a-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="7311a-104">Ви – Глобальний адміністратор у каталозі.</span><span class="sxs-lookup"><span data-stu-id="7311a-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="7311a-105">Ви не ввійшли в обліковий запис, який містить каталог за замовчуванням, як-от contoso.onmicrosoft.com у підписаних облікових записів, як-от admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="7311a-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="7311a-106">Видаліть усі активні програми в каталозі перед видаленням.</span><span class="sxs-lookup"><span data-stu-id="7311a-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="7311a-107">Щоб видалити активні програми, перейдіть до реєстрацій програм і видаліть вже наведені програми.</span><span class="sxs-lookup"><span data-stu-id="7311a-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="7311a-108">Немає активних передплат для будь-яких служб Microsoft Online, таких як Microsoft Azure, Office 365 або Azure AD Premium, пов'язані з каталогом.</span><span class="sxs-lookup"><span data-stu-id="7311a-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="7311a-109">Передача передплати або прискорення скасування активної передплати за допомогою служби Azure та виставлення рахунків.</span><span class="sxs-lookup"><span data-stu-id="7311a-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="7311a-110">Дізнайтеся більше про те, як скасувати передплату Office 365 і Azure.</span><span class="sxs-lookup"><span data-stu-id="7311a-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="7311a-111">Щоб отримати вказівки щодо зв'язування або додавання наявної передплатою до клієнта, зверніться до статті [зв'язати або додайте до свого клієнта Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="7311a-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="7311a-112">Немає активної ліцензії.</span><span class="sxs-lookup"><span data-stu-id="7311a-112">There are no Active license.</span></span> <span data-ttu-id="7311a-113">Щоб видалити ліцензії, Дізнайтеся, [як видалити ліцензію](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="7311a-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="7311a-114">У каталозі немає інших активних користувачів, крім себе, як Глобальний адміністратор, коли ви намагаєтеся видалити Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7311a-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="7311a-115">Видаліть будь-які інші активні користувачі та всі залежності від настроюваного імені домену в клієнті також повинні бути видалені, наприклад користувачі, створені за допомогою admin@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="7311a-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="7311a-116">Докладні відомості про те, як виконати наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="7311a-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="7311a-117">Видаліть "Azure Active Directory" або "Передплата", перегляньте статтю [DELETE Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="7311a-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="7311a-118">Видаліть програми в каталозі, перегляньте статтю [видалення програм](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="7311a-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
