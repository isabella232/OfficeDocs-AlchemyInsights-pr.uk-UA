---
title: Надбудова "команди" для Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630023"
---
# <a name="teams-add-in-for-mac"></a>Надбудова "команди" для Mac

Щоб виправити неполадки в надбудові відсутніх груп для користувачів операційної системи Mac, виконайте наведені нижче дії.

**Крок 1:** Якщо у вас є гібридний локальний Exchange (2016 CU3 або пізніша версія), скористайтеся засобом Test-HMA.ps1, щоб підтвердити, що ця гібридна сучасна автентифікація правильно настроєно. Докладні відомості наведено в статті [перевірка гібридної версії сучасної автентифікації для програми Outlook для IOS і Android](https://aka.ms/AA980zq).  

**Примітка** . Використовуйте формат адреси для UPN (наприклад, [username@contoso.com](mailto:username@contoso.com)), а не домен \ ім'я _ користувача. Зробіть це навіть для користувачів із поштовими скриньками Exchange Online.

**Крок 2:** Маєте користувача перейти до **Tools**  >  **облікових записів**Tools... у програмі Outlook для Mac і знайдіть і виберіть обліковий запис. Переконайтеся, що ім'я користувача вказано в форматі UPN (наприклад, [username@contoso.com](mailto:username@contoso.com)).

**Крок 3:** Підтвердьте, що користувач – це ліцензований користувач групи Microsoft. Користувач має використовувати передплатою Office 365 для Mac, версію продукту 16,24 або пізнішу.