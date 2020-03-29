---
title: Остаточне видалення сайту в SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955232"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="74b8c-102">Остаточне видалення сайту в SharePoint</span><span class="sxs-lookup"><span data-stu-id="74b8c-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="74b8c-103">Щоб повторно використати URL-адресу видаленого сайту (для повторного створення сайту) або остаточно видалити сайт, який більше не використовується, можна скористатися командою **Остаточно видалити** в новому Центрі адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="74b8c-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="74b8c-104">Відкрийте [сторінку "Видалені сайти" в новому Центрі адміністрування SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) і ввійдіть за допомогою облікового запису з дозволами адміністратора для вашої організації.</span><span class="sxs-lookup"><span data-stu-id="74b8c-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="74b8c-105">У лівому стовпці виберіть сайт. </span><span class="sxs-lookup"><span data-stu-id="74b8c-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="74b8c-106">Клацніть **Остаточно видалити**.</span><span class="sxs-lookup"><span data-stu-id="74b8c-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="74b8c-107">**Примітка.** Сайти, підключені до групи, не можна остаточно видалити з нового Центру адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="74b8c-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="74b8c-108">Натомість потрібно скористатися командою [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="74b8c-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="74b8c-109">Докладні відомості див. в статті [Остаточне видалення сайту](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="74b8c-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
