---
title: Проблеми з реєстрацією в власників програм
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405325"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="29899-102">Проблеми з реєстрацією в власників програм</span><span class="sxs-lookup"><span data-stu-id="29899-102">App Registration Owner issues</span></span>

<span data-ttu-id="29899-103">Нижче наведено доступні способи додавання учасників як власників для реєстрації програм.</span><span class="sxs-lookup"><span data-stu-id="29899-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="29899-104">Використання модуля Azure AD PowerShell</span><span class="sxs-lookup"><span data-stu-id="29899-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="29899-105">[Довідник: Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="29899-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="29899-106">Використання Azure CLI – `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="29899-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="29899-107">Довідка: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="29899-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="29899-108">Використання MS Graph –</span><span class="sxs-lookup"><span data-stu-id="29899-108">Using MS Graph -</span></span>

    <span data-ttu-id="29899-109">Довідник: [додавання власника – Microsoft Graph 1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="29899-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="29899-110">Використання порталу Azure AD. Перейдіть до portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > Реєстрації програм > Виберіть свою програму для > власників > Додати власників</span><span class="sxs-lookup"><span data-stu-id="29899-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="29899-111">**Не вдається переглянути програму на надписах реєстрації програм, навіть якщо ви – власник цієї програми?**</span><span class="sxs-lookup"><span data-stu-id="29899-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="29899-112">Власник програми не є адміністративною роллю.</span><span class="sxs-lookup"><span data-stu-id="29899-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="29899-113">Якщо параметр [Обмежити доступ](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) до порталу адміністрування Azure AD ввімкнуто, переглядати програми на порталі реєстрації програм зможе лише адміністратор.</span><span class="sxs-lookup"><span data-stu-id="29899-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="29899-114">Щоб власник зможе переглядати програми, вимкніть цей параметр (установіть значення "Ні") або призначте роль адміністратора власнику лише для конкретної програми.</span><span class="sxs-lookup"><span data-stu-id="29899-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="29899-115">Однак для цього потрібно мати ліцензію Azure AD Premium P2 та ввімкнути [керування привілейованими ідентичноями.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="29899-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
