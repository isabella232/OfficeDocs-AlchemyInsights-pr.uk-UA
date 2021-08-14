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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923665"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Коли зміни профілю синхронізуються з програмою SharePoint профілів користувачів?

SharePoint Онлайн використовує завдання таймера імпорту Active Directory (імпорт AD), щоб імпортувати користувачів і групи до програми профілю користувача. 
  
1. Під час імпорту AD синхронізуються зміни з SharePoint Online Directory Store із програмою профілю користувача. Ці зміни обробляються пакетами.
    
2. Завдання таймера виконується, доки не буде синхронізовано зміни.
    
> [!NOTE]
> Час, необхідний для виконання завдання, залежить від кількості змін в процесі. Велика кількість змін триватиме довше. У угоді про рівень послуг (SLA) указується, що зміна користувача в каталозі SharePoint Online відображатимуться в програмі профілю користувача протягом 24 годин. 
  
[Докладні відомості про синхронізацію профілю користувача в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

