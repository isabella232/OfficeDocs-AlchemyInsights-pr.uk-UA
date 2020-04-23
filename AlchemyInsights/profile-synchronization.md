---
title: Синхронізація профілів
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768134"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Коли мій профіль змінює синхронізацію з додатком профілю користувача SharePoint?

SharePoint Online використовує завдання таймера імпорту Active Directory (імпорт ОГОЛОШЕНЬ) для імпорту користувачів і груп до застосунку профілю користувача. 
  
1. AD імпорту синхронізує зміни з магазину SharePoint Online каталогу до застосунку профілю користувача. Ці зміни обробляються пакетів.
    
2. Завдання таймера запускається, доки зміни не буде синхронізовано.
    
> [!NOTE]
> Час, необхідний для запуску завдання, залежить від кількості змін, які потрібно обробити. Велика кількість змін триває довше. Угода про рівень послуг (SLA) стверджує, що зміна користувача в каталозі SharePoint Online буде відображена в додатку профілю користувача за 24 години. 
  
[Додаткові відомості про синхронізацію профілів користувачів у SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

