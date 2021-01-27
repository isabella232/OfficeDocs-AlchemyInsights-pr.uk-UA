---
title: Видалення або відновлення програм
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015022"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="73d8b-102">Видалення або відновлення програм</span><span class="sxs-lookup"><span data-stu-id="73d8b-102">Delete or restore applications</span></span>

<span data-ttu-id="73d8b-103">**Щоб видалити програму зі свого клієнта Azure AD**, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="73d8b-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="73d8b-104">На **порталі Лазурне AD** виберіть елемент **корпоративні програми**.</span><span class="sxs-lookup"><span data-stu-id="73d8b-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="73d8b-105">Потім знайдіть і виберіть програму, яку потрібно видалити.</span><span class="sxs-lookup"><span data-stu-id="73d8b-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="73d8b-106">У розділі **керування** в області ліворуч виберіть **Властивості**.</span><span class="sxs-lookup"><span data-stu-id="73d8b-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="73d8b-107">Натисніть кнопку **Видалити**, а потім натисніть кнопку **так** , щоб підтвердити видалення програми зі свого клієнта Azure AD.</span><span class="sxs-lookup"><span data-stu-id="73d8b-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="73d8b-108">Докладні відомості про видалення програми наведено в статті [QuickStart: видалення програми зі свого клієнта Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="73d8b-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="73d8b-109">У PowerShell цей командлет DELETE [-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) видаляє конфігурації проксі-сервера програми з певної програми в лазуровому Active Directory та може видалити програму повністю, якщо це вказано.</span><span class="sxs-lookup"><span data-stu-id="73d8b-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="73d8b-110">Ви можете **відновити видалену програму** за допомогою PowerShell.</span><span class="sxs-lookup"><span data-stu-id="73d8b-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="73d8b-111">Після того, як програма, яку потрібно відновити, була виявлена, її можна відновити за допомогою функції [відновлення – AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="73d8b-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
