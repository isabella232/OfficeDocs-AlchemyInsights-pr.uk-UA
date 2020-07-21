---
title: Один користувач, не бачачи надбудови, у програмі Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198224"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="7d2d3-102">Один користувач, не бачачи надбудови, у програмі Outlook</span><span class="sxs-lookup"><span data-stu-id="7d2d3-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="7d2d3-103">Користувач може бути частиною ролі, яка не має правильний AppsForOfficeEnabled параметр.</span><span class="sxs-lookup"><span data-stu-id="7d2d3-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="7d2d3-104">Запустити цю команду, щоб дізнатися, чи правильну роль пов'язано з користувачем:</span><span class="sxs-lookup"><span data-stu-id="7d2d3-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="7d2d3-105">Get-Управліннярольові призначення-RoleAssignee user@domain.com-делегування $false | Формат таблиці-роль авто, ім'я _ сторінки, Ролізинсінетип</span><span class="sxs-lookup"><span data-stu-id="7d2d3-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="7d2d3-106">Щоб дізнатися більше, перегляньте відомості про [указання адміністраторів і користувачів, які можуть інсталювати надбудови Outlook і керувати ними](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="7d2d3-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
