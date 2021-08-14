---
title: Власник не може створювати вкладену папку за допомогою Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063145"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Власник не може створювати вкладену папку за допомогою Outlook

**Власники спільних папок можуть створювати вкладені папки за допомогою Outlook. Цю проблему буде вирішено незабаром.**

Тим часом скористайтеся одним із наведених нижче способів вирішення.

1. Використовуйте Outlook для Mac, щоб створити вкладену систему, оскільки ця проблема виникає лише в Outlook для настільних комп'ютерів (усіх версій)
2. Адміністратор може створити вкладену адресу за допомогою EXO Shell або EAC
3. Змінення параметра DefaultPublicFolderMailbox/EffectivePublicFolderMailbox користувача на іншу поштову скриньку, відмінну від поштової скриньки вмісту папки, яка виникає, коли проблема виникає  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Зачекайте годину, перезапустіть клієнт Outlook