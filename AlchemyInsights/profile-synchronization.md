---
title: Синхронізація профілю
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320730"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Коли зміни профілю синхронізуються з програмою SharePoint профілів користувачів?

SharePoint Онлайн використовує завдання таймера імпорту Active Directory (імпорт AD), щоб імпортувати користувачів і групи до програми профілю користувача. 
  
1. Під час імпорту AD синхронізуються зміни з SharePoint Online Directory Store із програмою профілю користувача. Ці зміни обробляються пакетами.
    
2. Завдання таймера виконується, доки не буде синхронізовано зміни.
    
**Примітка.** Час, необхідний для запуску завдання, залежить від кількості змін, які потрібно обробити. Велика кількість змін триватиме довше. У угоді про рівень послуг (SLA) указується, що зміна користувача в каталозі SharePoint Online відображатимуться в програмі профілю користувача протягом 24 годин. 
  
[Докладні відомості про синхронізацію профілю користувача в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

