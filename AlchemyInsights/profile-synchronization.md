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
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372005"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Коли мої зміни профілю синхронізації застосунку профілю користувача SharePoint?

SharePoint Online використовує Active Directory імпортувати таймера (оголошення імпорту) для імпорту користувачів і груп у застосунку профілю користувача. 
  
1. Оголошення імпорту синхронізує зміни з магазину каталозі на сайті SharePoint до застосунку профілів користувачів. Ці зміни не будуть оброблені партіями.
    
2. Завдання таймера керує поки синхронізації змін.
    
> [!NOTE]
> Тривалість завдання працювати залежить від кількості змін для обробки. Велику кількість змін займає більше часу. Угоди про рівень обслуговування (SLA) стверджує, що зміна користувачеві у SharePoint Інтернет-каталог також буде застосовано до застосунку профілю користувача в 24 годин. 
  
[Детальніше про службу синхронізації профілів користувачів у SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

