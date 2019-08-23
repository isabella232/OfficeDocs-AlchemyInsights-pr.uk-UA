---
title: Профіль синхронізації
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554354"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="babb5-102">Коли мої зміни профілю синхронізації застосунку профілю користувача SharePoint?</span><span class="sxs-lookup"><span data-stu-id="babb5-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="babb5-103">SharePoint Online використовує Active Directory імпортувати таймера (оголошення імпорту) для імпорту користувачів і груп у застосунку профілю користувача.</span><span class="sxs-lookup"><span data-stu-id="babb5-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="babb5-104">Оголошення імпорту синхронізує зміни з магазину каталозі на сайті SharePoint до застосунку профілів користувачів.</span><span class="sxs-lookup"><span data-stu-id="babb5-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="babb5-105">Ці зміни не будуть оброблені партіями.</span><span class="sxs-lookup"><span data-stu-id="babb5-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="babb5-106">Завдання таймера керує поки синхронізації змін.</span><span class="sxs-lookup"><span data-stu-id="babb5-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="babb5-107">Тривалість завдання працювати залежить від кількості змін для обробки.</span><span class="sxs-lookup"><span data-stu-id="babb5-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="babb5-108">Велику кількість змін займає більше часу.</span><span class="sxs-lookup"><span data-stu-id="babb5-108">A large number of changes takes longer.</span></span> <span data-ttu-id="babb5-109">Угоди про рівень обслуговування (SLA) стверджує, що зміна користувачеві у SharePoint Інтернет-каталог також буде застосовано до застосунку профілю користувача в 24 годин.</span><span class="sxs-lookup"><span data-stu-id="babb5-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="babb5-110">Детальніше про службу синхронізації профілів користувачів у SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="babb5-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

