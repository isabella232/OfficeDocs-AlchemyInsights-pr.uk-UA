---
title: Кілька користувачів отримати доступ відмовлено помилка під час додавання надбудови в Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424179"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Кілька користувачів отримати доступ відмовлено помилка під час додавання надбудови в Outlook

Можна вказати, які адміністратори в організації мають дозволи на інсталяцію та керування надбудовами для Outlook. Також можна вказати, які користувачі в організації мають дозвіл на інсталяцію та керування надбудовами для власного використання.

Докладніше, перегляньте відомості про [указання адміністраторів і користувачів, які можуть інсталювати надбудови Outlook і керувати ними](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Щоб переконатися, що ви успішно призначені дозволи для користувача, замініть <Role Name> ім'я ролі, щоб перевірити і виконайте таку команду в Exchange Online PowerShell:

Get-Управліннярольова призначення-роль " <Role Name> "-geteffectiveusers

У цьому прикладі пояснюється, як перевірити, кому призначено дозволи на інсталяцію надбудов із магазину Office для організації.

Powershell

-Роль "org-Marketplace додатків"-GetEffectiveUsers

У результатах пошуку Get-Управліннярольова призначення, перегляньте записи в стовпці ефективні користувачі.

Докладні відомості про синтаксис і [параметр див.](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)
 