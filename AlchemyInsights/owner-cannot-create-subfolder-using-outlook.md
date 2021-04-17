---
title: Власник не може створити вкладену папку за допомогою Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836156"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Власник не може створити вкладену папку за допомогою Outlook

**Власники спільних папок, які створюють вкладені папки за допомогою Outlook, можуть виникати незмінні проблеми. Цю проблему буде вирішено незабаром.**

Тим часом скористайтеся одним із наведених нижче способів вирішення.

1. Створення вкладеної папки в Outlook для Mac, оскільки ця проблема виникає лише в Outlook для настільних комп'ютерів (усі версії)
2. Адміністратор може створити вкладену адресу за допомогою EXO Shell або EAC
3. Змінення параметра DefaultPublicFolderMailbox/EffectivePublicFolderMailbox користувача на іншу поштову скриньку, відмінну від поштової скриньки вмісту папки, яка виникає, коли проблема виникає  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Зачекайте годину, перезапустіть клієнт Outlook