---
title: Спільний доступ із зовнішніми користувачами не працює
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43913023"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="401e3-102">Вирішення проблем з доступом до вмісту SharePoint із зовнішніми користувачами</span><span class="sxs-lookup"><span data-stu-id="401e3-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="401e3-103">Переконайтеся, що для вашої організації увімкнуто зовнішній спільний доступ:</span><span class="sxs-lookup"><span data-stu-id="401e3-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="401e3-104">Перейдіть до [сторінки надбудови &amp; служб у центрі адміністрування Microsoft 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)і натисніть кнопку **сайти**.</span><span class="sxs-lookup"><span data-stu-id="401e3-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="401e3-105">Переконайтеся, що параметр увімкнено "увімкнено".</span><span class="sxs-lookup"><span data-stu-id="401e3-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="401e3-106">Якщо вибрано "лише існуючі зовнішні користувачі", переконайтеся, що зовнішній користувач у списку Центр адміністрування Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="401e3-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="401e3-107">Переконайтеся, що зовнішній спільний доступ увімкнуто для цього сайту.</span><span class="sxs-lookup"><span data-stu-id="401e3-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="401e3-108">Для класичної колекції сайтів:</span><span class="sxs-lookup"><span data-stu-id="401e3-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="401e3-109">У новому центрі адміністрування SharePoint на лівій панелі виберіть пункт **сайти**.</span><span class="sxs-lookup"><span data-stu-id="401e3-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="401e3-110">Виберіть сайт або сайти, а на стрічці натисніть **спільний доступ**.</span><span class="sxs-lookup"><span data-stu-id="401e3-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="401e3-111">Для команди сайту, який належить до групи Microsoft 365 або сайту зв'язку:</span><span class="sxs-lookup"><span data-stu-id="401e3-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="401e3-112">Ці нові типи сайтів мають однакові настройки спільного доступу, що й для всієї організації, якщо настройки для всієї організації дають змогу обмінюватися файлами за допомогою посилань, які не потребують входу.</span><span class="sxs-lookup"><span data-stu-id="401e3-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="401e3-113">У цьому випадку сайти дозволяють обмінюватися з новими та існуючими зовнішніми користувачами, які ввійшли в обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="401e3-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="401e3-114">Щоб змінити настройки для певних сайтів, використовуйте новий Центр адміністрування SharePoint або PowerShell.</span><span class="sxs-lookup"><span data-stu-id="401e3-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="401e3-115">[Докладні відомості](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="401e3-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="401e3-116">Настройка зовнішнього спільного доступу для будь-якого сайту може бути більш обмежувальною, ніж настройка для всієї організації, але не більш дозвільна, ніж настройка організації.</span><span class="sxs-lookup"><span data-stu-id="401e3-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

