---
title: Остаточне видалення сайту в SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944332"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Остаточне видалення сайту в SharePoint

Щоб повторно використати URL-адресу видаленого сайту (для повторного створення сайту) або остаточно видалити сайт, який більше не використовується, можна скористатися командою **Остаточно видалити** в новому Центрі адміністрування SharePoint. 

1. Відкрийте [сторінку "Видалені сайти" в новому Центрі адміністрування SharePoint](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) і ввійдіть за допомогою облікового запису з дозволами адміністратора для вашої організації. 

2. У лівому стовпці виберіть сайт.  

3. Клацніть **Остаточно видалити**. 

**Примітка.** Сайти, підключені до групи, не можна остаточно видалити з нового Центру адміністрування SharePoint. Натомість потрібно скористатися командою [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Докладні відомості див. в статті [Остаточне видалення сайту](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
