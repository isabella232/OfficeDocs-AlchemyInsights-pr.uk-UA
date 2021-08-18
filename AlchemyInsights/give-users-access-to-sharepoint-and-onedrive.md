---
title: Надання користувачам доступу до SharePoint та OneDrive
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
ms.openlocfilehash: 8c27997b1bca1d47ad876a0a6941607517912333
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58333144"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a>Надання користувачам доступу до SharePoint та OneDrive

**Примітка.** Якщо сайт OneDrive або SharePoint недоступний для кількох користувачів, які раніше мали доступ, може виникнути тимчасова проблема з обслуговуванням. [Перевірка приладної дошки справності служби](https://portal.office.com/adminportal/home#/servicehealth)
  
Якщо потрібно, щоб користувачі у вашій організації могли входити в SharePoint і OneDrive, потрібно додати для них облікові записи та переконатися, що вони мають ліцензію, яка надає їм доступ до SharePoint і OneDrive. Найпростіший спосіб додати користувачів – це зробити Центр адміністрування Microsoft 365.
  
1. На сторінці [Активні користувачі в Центр адміністрування Microsoft 365](https://portal.office.com/adminportal/home#/users)натисніть кнопку Додати **користувача.**
    
2. Введіть відомості про користувача та переконайтеся, що в розділі Ліцензії на продукт вибрано ліцензію, **а SharePoint Онлайн.** 
    
Зверніть увагу: якщо надати спільний доступ зовнішнім користувачам в організації, SharePoint надати спільний доступ до OneDrive спільний доступ користувачам поза межами організації. Надавати ліцензії зовнішнім користувачам не потрібно. Крім того, додавати облікові записи для них не потрібно, якщо для параметра спільного доступу встановлено значення "Лише наявні зовнішні користувачі". У такому разі, якщо користувачів немає в каталозі вашої організації, їх потрібно додати як користувачів-гостей у Центрі адміністрування Azure AD.
  

