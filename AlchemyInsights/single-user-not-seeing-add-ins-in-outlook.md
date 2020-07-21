---
title: Один користувач, не бачачи надбудови, у програмі Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198224"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Один користувач, не бачачи надбудови, у програмі Outlook

Користувач може бути частиною ролі, яка не має правильний AppsForOfficeEnabled параметр. Запустити цю команду, щоб дізнатися, чи правильну роль пов'язано з користувачем:

Get-Управліннярольові призначення-RoleAssignee user@domain.com-делегування $false | Формат таблиці-роль авто, ім'я _ сторінки, Ролізинсінетип

Щоб дізнатися більше, перегляньте відомості про [указання адміністраторів і користувачів, які можуть інсталювати надбудови Outlook і керувати ними](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
