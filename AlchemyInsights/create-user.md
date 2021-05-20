---
title: Створення користувача
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569768"
---
# <a name="create-user"></a><span data-ttu-id="da5dd-102">Створення користувача</span><span class="sxs-lookup"><span data-stu-id="da5dd-102">Create user</span></span>

<span data-ttu-id="da5dd-103">**ОГОЛОШЕННЯ:**</span><span class="sxs-lookup"><span data-stu-id="da5dd-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="da5dd-104">[Вилучення підтримки входу в WebView від Google із 4 січня 2021 р.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="da5dd-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="da5dd-105">Перевірте, чи можуть на ваші програми вплинути наведені в [Google](https://go.microsoft.com/fwlink/?linkid=2157323) указівки щодо сумісності тестування.</span><span class="sxs-lookup"><span data-stu-id="da5dd-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="da5dd-106">Увійдіть у систему за допомогою облікових записів Google споживачів і переконайтеся, що ви використовуєте системний веб-браузер або системний браузер.</span><span class="sxs-lookup"><span data-stu-id="da5dd-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="da5dd-107">Докладні відомості див. в статтях Проблеми із входом лише в програми [за допомогою браузера Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="da5dd-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="da5dd-108">**Не вдається створити нового користувача в каталозі Azure AD**</span><span class="sxs-lookup"><span data-stu-id="da5dd-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="da5dd-109">Переконайтеся, що ви маєте право створювати нового стандартного користувача.</span><span class="sxs-lookup"><span data-stu-id="da5dd-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="da5dd-110">Створити нового стандартного користувача може лише роль глобального адміністратора або Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="da5dd-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="da5dd-111">Якщо ви не на одній із цих ролей, попросіть адміністратора додати вас до однієї з цих ролей або створити новий обліковий запис користувача для вас.</span><span class="sxs-lookup"><span data-stu-id="da5dd-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="da5dd-112">Переконайтеся, що ім'я користувача перевірено в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da5dd-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="da5dd-113">Якщо в Azure AD немає перевірених імен настроюваних доменів, можна використовувати початковий домен Azure AD, який закінчується на \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="da5dd-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="da5dd-114">Переконайтеся, що ім'я користувача в домені, не ітерованому до Azure AD, з локальної служби AD.</span><span class="sxs-lookup"><span data-stu-id="da5dd-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="da5dd-115">Користувачів не можна додавати до хмари з іменами доменів, іфедеративними з локальних доменів.</span><span class="sxs-lookup"><span data-stu-id="da5dd-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="da5dd-116">Переконайтеся, що жодний інший користувач або контакт не має імені користувача, яке потрібно призначити новому користувачу.</span><span class="sxs-lookup"><span data-stu-id="da5dd-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="da5dd-117">Імена користувачів мають бути унікальні в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da5dd-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="da5dd-118">Див. [номери ролей і адміністраторів Azure AD](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da5dd-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="da5dd-119">Перегляньте [імена доменів](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) для azure AD.</span><span class="sxs-lookup"><span data-stu-id="da5dd-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="da5dd-120">Перегляньте [контрольні журнали,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) щоб переглянути докладніші відомості про нещодавно створеного або видаленого користувача (наприклад, тих, хто виконав дію) і час.</span><span class="sxs-lookup"><span data-stu-id="da5dd-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="da5dd-121">Докладні відомості про додавання нових користувачів див. в цій [статтях.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="da5dd-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="da5dd-122">[Права адміністратора Azure AD: дозволи](/azure/active-directory/active-directory-assign-admin-roles)адміністратора в Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="da5dd-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="da5dd-123">Ви також можете [створити нового користувача за допомогою Azure AD PowerShell.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="da5dd-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
