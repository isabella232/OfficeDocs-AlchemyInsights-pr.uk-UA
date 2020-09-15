---
title: Надання користувачам доступу до SharePoint і OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677228"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="e297c-102">Надання користувачам доступу до SharePoint і OneDrive</span><span class="sxs-lookup"><span data-stu-id="e297c-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="e297c-103">Якщо ви не маєте доступу до кількох користувачів, які раніше мали доступ до служби "OneDrive" або сайту SharePoint, може виникнути тимчасова проблема з обслуговуванням.</span><span class="sxs-lookup"><span data-stu-id="e297c-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="e297c-104">Перевірка приладної дошки справності служби</span><span class="sxs-lookup"><span data-stu-id="e297c-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="e297c-105">Якщо ви хочете, щоб користувачі в організації могли входити в службу SharePoint і OneDrive, потрібно додати облікові записи та переконатися, що вони мають ліцензію, яка надає їм доступ до SharePoint і OneDrive.</span><span class="sxs-lookup"><span data-stu-id="e297c-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="e297c-106">Найпростіший спосіб додати користувачів до центру адміністрування Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e297c-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="e297c-107">Перейдіть на [сторінку активні користувачі в центрі адміністрування Microsoft 365](https://portal.office.com/adminportal/home#/users)і виберіть пункт **Додати користувача**.</span><span class="sxs-lookup"><span data-stu-id="e297c-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="e297c-108">Введіть відомості для користувача та переконайтеся, що в розділі **ліцензії на продукти**призначено ліцензію, і вибрано службу **SharePoint Online** .</span><span class="sxs-lookup"><span data-stu-id="e297c-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="e297c-109">Зверніть увагу, що якщо дозволити зовнішнім спільним доступом у вашій організації, користувачі можуть надавати спільний доступ до вмісту SharePoint і OneDrive користувачам за межами організації.</span><span class="sxs-lookup"><span data-stu-id="e297c-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="e297c-110">Не потрібно надавати ці зовнішні ліцензії для користувачів.</span><span class="sxs-lookup"><span data-stu-id="e297c-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="e297c-111">Крім того, для них не потрібно додавати облікові записи, якщо для спільного доступу встановлено значення "лише наявний зовнішній користувач".</span><span class="sxs-lookup"><span data-stu-id="e297c-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="e297c-112">У такому випадку, якщо користувачі не входять до каталогу вашої організації, їх потрібно додати як гостьові користувачі в центрі адміністрування Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e297c-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

