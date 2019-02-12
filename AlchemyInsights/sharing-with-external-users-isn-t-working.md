---
title: Спільно з зовнішніми користувачами не працює
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900914"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="f46bf-102">Виправлення неполадок із обміну вміст SharePoint із зовнішніми користувачами</span><span class="sxs-lookup"><span data-stu-id="f46bf-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="f46bf-103">Переконайтеся, що зовнішній ввімкнення спільного доступу для вашої організації:</span><span class="sxs-lookup"><span data-stu-id="f46bf-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="f46bf-104">Зайдіть на [послуги &amp; надбудови для сторінки центру адміністрування служби Office 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)і натисніть кнопку **сайти**.</span><span class="sxs-lookup"><span data-stu-id="f46bf-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="f46bf-p101">Переконайтеся, що параметр звернений "Вкл." Якщо вибрано "Тільки існуючі зовнішніх користувачів", переконайтеся, що зовнішнім користувачем перераховані центру адміністрування служби Office 365.</span><span class="sxs-lookup"><span data-stu-id="f46bf-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="f46bf-p102">Переконайтеся, що зовнішні зрівнялася ввімкнуто для сайту. Для колекції Класичні сайтів:</span><span class="sxs-lookup"><span data-stu-id="f46bf-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="f46bf-109">Класичний центру адміністрування SharePoint, на панелі ліворуч натисніть **колекцій сайтів**.</span><span class="sxs-lookup"><span data-stu-id="f46bf-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="f46bf-110">Виберіть сайт або сайти і на стрічці клацніть **спільний доступ**.</span><span class="sxs-lookup"><span data-stu-id="f46bf-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="f46bf-111">Для сайту групи, що належить до групи Office 365, або повідомлення сайту:</span><span class="sxs-lookup"><span data-stu-id="f46bf-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="f46bf-p103">Ці нові типи сайту мають ж обміну налаштування як ваші налаштування всієї організації, якщо налаштування всієї організації дозволяє спільне використання файлів за допомогою посилань, які не потребують входу. У такому випадку сайти вносили з існуючих та зовнішні користувачі, які входу. Щоб змінити настройки для певних сайтів, за допомогою нового центру адміністрування SharePoint (preview) або PowerShell. [Докладніше](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="f46bf-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="f46bf-116">Зовнішня настройка спільного доступу для будь-якого сайту може бути більш обмежувальним, ніж ваші налаштування всієї організації, але не більш сприятливий ніж налаштування всієї організації.</span><span class="sxs-lookup"><span data-stu-id="f46bf-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

