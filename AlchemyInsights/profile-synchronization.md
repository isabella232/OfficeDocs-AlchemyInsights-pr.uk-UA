---
title: Профіль синхронізації
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28319246"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="4ef6e-102">Коли мої зміни профілю синхронізації застосунку профілю користувача SharePoint?</span><span class="sxs-lookup"><span data-stu-id="4ef6e-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="4ef6e-103">SharePoint Online використовує Active Directory імпортувати таймера (оголошення імпорту) для імпорту користувачів і груп у застосунку профілю користувача.</span><span class="sxs-lookup"><span data-stu-id="4ef6e-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="4ef6e-p101">Оголошення імпорту синхронізує зміни з магазину каталозі на сайті SharePoint до застосунку профілів користувачів. Ці зміни не будуть оброблені партіями.</span><span class="sxs-lookup"><span data-stu-id="4ef6e-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="4ef6e-106">Завдання таймера керує поки синхронізації змін.</span><span class="sxs-lookup"><span data-stu-id="4ef6e-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="4ef6e-p102">Тривалість завдання працювати залежить від кількості змін для обробки. Велику кількість змін займає більше часу. Угоди про рівень обслуговування (SLA) стверджує, що зміна користувачеві у SharePoint Інтернет-каталог також буде застосовано до застосунку профілю користувача в 24 годин.</span><span class="sxs-lookup"><span data-stu-id="4ef6e-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="4ef6e-110">Детальніше про службу синхронізації профілів користувачів у SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4ef6e-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

