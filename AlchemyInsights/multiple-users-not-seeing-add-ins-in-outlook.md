---
title: Кілька користувачів, які не бачать надбудови, у програмі Outlook
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198246"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Кілька користувачів, які не бачать надбудови, у програмі Outlook

Якщо перевірити Outlook надбудови і не відображаються, як перший крок для виправлення неполадок, використовуйте командлет **Get-Організаціїconfig** PowerShell запит _Appsforofficeenabled_ параметр. Якщо запит повертає значення **false**, установіть цей параметр **True** за допомогою командлета **Set-організаціїconfig** , тому надбудови відображаються належним чином.

Ми не рекомендуємо, що _Appsforofficeenabled_ параметр значення **false**. Значення **false** скасовує всі вищевикладені адміністративні та настройки ролей користувача і запобігає активації будь-якого користувача в організації будь-які нові програми.

Для отримання додаткових відомостей див. [зазначення адміністраторів і користувачів, які можуть інсталювати надбудови Outlook і керувати ними](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).