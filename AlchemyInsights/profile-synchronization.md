---
title: Синхронізація профілів
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: eee1080a95955332e205db3852381e39aaf5ae0e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801790"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Коли мій профіль змінює синхронізацію в застосунку профілю користувача SharePoint?

Служба SharePoint Online використовує завдання таймера імпорту Active Directory (імпорт оголошення), щоб імпортувати користувачів і групи в програму профілю користувача. 
  
1. Імпорт AD синхронізує зміни з магазину каталогів SharePoint Online до застосунку профілю користувача. Ці зміни обробляються в партіях.
    
2. Завдання таймера запускається, доки зміни не буде синхронізовано.
    
> [!NOTE]
> Час, потрібний для виконання завдання, залежить від кількості змін, внесених до процесу. Велика кількість змін триває довше. Угода про рівень служби (SLA) заявляє, що змінення користувача в каталозі SharePoint Online буде відображено в програмі профілю користувача протягом 24 годин. 
  
[Докладні відомості про синхронізацію профілів користувачів у службі SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

