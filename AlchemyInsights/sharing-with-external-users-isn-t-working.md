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
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: d4c8fc75ff8db2319b88a20bea9b3ee661f2e36e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36502252"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="30a01-102">Виправлення неполадок із обміну вміст SharePoint із зовнішніми користувачами</span><span class="sxs-lookup"><span data-stu-id="30a01-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="30a01-103">Переконайтеся, що зовнішній ввімкнення спільного доступу для вашої організації:</span><span class="sxs-lookup"><span data-stu-id="30a01-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="30a01-104">Зайдіть на [послуги &amp; надбудови для сторінки центру адміністрування Microsoft Outlook 365](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)та натисніть кнопку **сайти**.</span><span class="sxs-lookup"><span data-stu-id="30a01-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="30a01-105">Переконайтеся, що параметр звернений "Вкл."</span><span class="sxs-lookup"><span data-stu-id="30a01-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="30a01-106">Якщо вибрано "Тільки існуючі зовнішніх користувачів", переконайтеся, що зовнішнім користувачем перераховані в Microsoft Outlook 365 центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="30a01-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="30a01-107">Переконайтеся, що зовнішні зрівнялася ввімкнуто для сайту.</span><span class="sxs-lookup"><span data-stu-id="30a01-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="30a01-108">Для колекції Класичні сайтів:</span><span class="sxs-lookup"><span data-stu-id="30a01-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="30a01-109">Нові центру адміністрування SharePoint, на лівій панелі натисніть кнопку **сайти**.</span><span class="sxs-lookup"><span data-stu-id="30a01-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="30a01-110">Виберіть сайт або сайти і на стрічці клацніть **спільний доступ**.</span><span class="sxs-lookup"><span data-stu-id="30a01-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="30a01-111">Для сайту групи, що належить до групи Office 365, або повідомлення сайту:</span><span class="sxs-lookup"><span data-stu-id="30a01-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="30a01-112">Ці нові типи сайту мають ж обміну налаштування як ваші налаштування всієї організації, якщо налаштування всієї організації дозволяє спільне використання файлів за допомогою посилань, які не потребують входу.</span><span class="sxs-lookup"><span data-stu-id="30a01-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="30a01-113">У такому випадку сайти вносили з існуючих та зовнішні користувачі, які входу.</span><span class="sxs-lookup"><span data-stu-id="30a01-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="30a01-114">Щоб змінити настройки для певних сайтів, за допомогою нового центру адміністрування SharePoint або PowerShell.</span><span class="sxs-lookup"><span data-stu-id="30a01-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="30a01-115">[Докладніше](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="30a01-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="30a01-116">Зовнішня настройка спільного доступу для будь-якого сайту може бути більш обмежувальним, ніж ваші налаштування всієї організації, але не більш сприятливий ніж налаштування всієї організації.</span><span class="sxs-lookup"><span data-stu-id="30a01-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

