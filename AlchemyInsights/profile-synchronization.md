---
title: Синхронізація профілів
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554354"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="89acd-102">Коли мій профіль змінює синхронізацію з додатком профілю користувача SharePoint?</span><span class="sxs-lookup"><span data-stu-id="89acd-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="89acd-103">SharePoint Online використовує завдання таймера імпорту Active Directory (імпорт ОГОЛОШЕНЬ) для імпорту користувачів і груп до застосунку профілю користувача.</span><span class="sxs-lookup"><span data-stu-id="89acd-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="89acd-104">AD імпорту синхронізує зміни з магазину SharePoint Online каталогу до застосунку профілю користувача.</span><span class="sxs-lookup"><span data-stu-id="89acd-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="89acd-105">Ці зміни обробляються пакетів.</span><span class="sxs-lookup"><span data-stu-id="89acd-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="89acd-106">Завдання таймера запускається, доки зміни не буде синхронізовано.</span><span class="sxs-lookup"><span data-stu-id="89acd-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="89acd-107">Час, необхідний для запуску завдання, залежить від кількості змін, які потрібно обробити.</span><span class="sxs-lookup"><span data-stu-id="89acd-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="89acd-108">Велика кількість змін триває довше.</span><span class="sxs-lookup"><span data-stu-id="89acd-108">A large number of changes takes longer.</span></span> <span data-ttu-id="89acd-109">Угода про рівень послуг (SLA) стверджує, що зміна користувача в каталозі SharePoint Online буде відображена в додатку профілю користувача за 24 години.</span><span class="sxs-lookup"><span data-stu-id="89acd-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="89acd-110">Додаткові відомості про синхронізацію профілів користувачів у SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="89acd-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

