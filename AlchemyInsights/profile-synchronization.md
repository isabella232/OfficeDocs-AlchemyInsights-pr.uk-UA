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
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Коли мій профіль змінює синхронізацію з додатком профілю користувача SharePoint?

SharePoint Online використовує завдання таймера імпорту Active Directory (імпорт ОГОЛОШЕНЬ) для імпорту користувачів і груп до застосунку профілю користувача. 
  
1. AD імпорту синхронізує зміни з магазину SharePoint Online каталогу до застосунку профілю користувача. Ці зміни обробляються пакетів.
    
2. Завдання таймера запускається, доки зміни не буде синхронізовано.
    
> [!NOTE]
> Час, необхідний для запуску завдання, залежить від кількості змін, які потрібно обробити. Велика кількість змін триває довше. Угода про рівень послуг (SLA) стверджує, що зміна користувача в каталозі SharePoint Online буде відображена в додатку профілю користувача за 24 години. 
  
[Додаткові відомості про синхронізацію профілів користувачів у SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

