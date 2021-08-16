---
title: Yammer проблем із ліцензуванням
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
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989756"
---
# <a name="yammer-licensing-issues"></a>Yammer проблем із ліцензуванням

Усі користувачі повинні мати ліцензію на використання Yammer Enterprise, але Yammer не вимагає, щоб користувачі мають ліцензію на доступ до служби. Якщо адміністратор змінить цей параметр, щоб заблокувати користувачів Microsoft 365 без Yammer, користувачі, які не мають ліцензії Yammer Enterprise, не мають доступу до Yammer служби. Докладні відомості [див. в Yammer керування ліцензіями користувачів Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Якщо видалити ліцензії в користувачів, плитка Yammer більше не відображається, а інші служби можуть скористатися вилученням ліцензій, щоб приховати функції. В інших випадках функції все ще можуть відображатися, але для роботи потрібно призначити ліцензію.  

**Ліцензія не оновлюється для користувача**  

Іноді користувачу призначається ліцензія, але й надалі не Yammer. Затримки частіше трапляються, коли виконується призначення масової ліцензії. Yammer користувачів може не оновлюватися в такому ж порядку, що й ліцензії, змінюються в Azure AD, оскільки система працює асинхронно. Зачекайте до 24 годин, перш ніж відкрити інцидент служби підтримки, щоб повідомити про проблеми синхронізації ліцензій.  

**Групове призначення ліцензій**  

Ліцензії можна призначати через Центр адміністрування або сценарії PowerShell. Докладні відомості див. [в статтях](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Призначення ліцензій користувачам і Призначення ліцензій обліковим записам користувачів за [допомогою Office 365 PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Служба підтримки Microsoft не надає допомоги зі створення сценаріїв, але доступна документація Yammer призначення ліцензій. Докладні відомості [див. в розділі Керування Yammer за допомогою Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).