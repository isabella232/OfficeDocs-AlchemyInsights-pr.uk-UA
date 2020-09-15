---
title: Надання користувачам доступу до SharePoint і OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677228"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Надання користувачам доступу до SharePoint і OneDrive

> [!NOTE]
> Якщо ви не маєте доступу до кількох користувачів, які раніше мали доступ до служби "OneDrive" або сайту SharePoint, може виникнути тимчасова проблема з обслуговуванням. [Перевірка приладної дошки справності служби](https://portal.office.com/adminportal/home#/servicehealth)
  
Якщо ви хочете, щоб користувачі в організації могли входити в службу SharePoint і OneDrive, потрібно додати облікові записи та переконатися, що вони мають ліцензію, яка надає їм доступ до SharePoint і OneDrive. Найпростіший спосіб додати користувачів до центру адміністрування Microsoft 365.
  
1. Перейдіть на [сторінку активні користувачі в центрі адміністрування Microsoft 365](https://portal.office.com/adminportal/home#/users)і виберіть пункт **Додати користувача**.
    
2. Введіть відомості для користувача та переконайтеся, що в розділі **ліцензії на продукти**призначено ліцензію, і вибрано службу **SharePoint Online** . 
    
Зверніть увагу, що якщо дозволити зовнішнім спільним доступом у вашій організації, користувачі можуть надавати спільний доступ до вмісту SharePoint і OneDrive користувачам за межами організації. Не потрібно надавати ці зовнішні ліцензії для користувачів. Крім того, для них не потрібно додавати облікові записи, якщо для спільного доступу встановлено значення "лише наявний зовнішній користувач". У такому випадку, якщо користувачі не входять до каталогу вашої організації, їх потрібно додати як гостьові користувачі в центрі адміністрування Azure AD.
  

