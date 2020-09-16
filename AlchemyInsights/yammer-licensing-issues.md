---
title: Проблеми з ліцензування Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657297"
---
# <a name="yammer-licensing-issues"></a>Проблеми з ліцензування Yammer

Усі користувачі повинні мати ліцензію на використання служби "Yammer Enterprise Service", але за замовчуванням Yammer не вимагає, щоб користувачі мали ліцензію на доступ до служби. Якщо адміністратор змінив параметр для блокування користувачів Microsoft 365 без ліцензій Yammer, користувачі, які не мають ліцензії Yammer Enterprise, не можуть отримати доступ до служби Yammer. Докладні відомості наведено в статті [керування ліцензіями користувачів Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Коли ліцензії буде видалено з користувачів, плитку Yammer більше не відображається, а інші служби можуть використовувати засіб видалення ліцензій, щоб приховати функції. В інших випадках функції все ще можуть відображатися, але для роботи з ним потрібно мати ліцензію.  

**Ліцензія не оновлюється для користувача**  

Час від часу користувача призначається ліцензія, але вона все ще не може отримати доступ до Yammer. Скоріш за все, після виконання завдання з масовою ліцензією відбувається затримка. Користувачі Yammer можуть не оновлюватись в тому ж порядку, що й ліцензії змінено в Azure AD, оскільки система працює асинхронно. Зачекайте до 24 годин, перш ніж відкрити інцидент підтримки, щоб повідомити про проблеми з синхронізацією ліцензії.  

**Масове призначення ліцензії**  

Ліцензії можна призначати через центр адміністрування або сценарії PowerShell. Докладні відомості наведено в статті [призначення ліцензій користувачам](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) і [призначення ліцензій для облікових записів користувачів із програмою Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Служба підтримки Microsoft не надає допомогу зі створення сценаріїв, але доступна документація до призначення ліцензії Yammer. Докладні відомості наведено в статті [керування ліцензіями Yammer за допомогою оболонки Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).