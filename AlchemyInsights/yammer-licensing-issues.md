---
title: Проблеми ліцензування Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148429"
---
# <a name="yammer-licensing-issues"></a>Проблеми ліцензування Yammer

Усі користувачі повинні мати ліцензію на використання служби Yammer Enterprise, але за промовчанням Yammer не вимагає, щоб користувачі мали ліцензію на доступ до служби. Коли адміністратор змінює параметр для блокування користувачів Microsoft 365 без ліцензій Yammer, користувачі, які не призначено ліцензією Yammer Enterprise, не можуть отримати доступ до служби Yammer. Щоб отримати додаткові відомості див. [керування ліцензіями користувача Yammer в Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Після того, як ліцензії, видаляються з користувачів, Yammer плитка більше не відображається, а також інші служби, можна використовувати ліцензії видалення приховати функції. В інших випадках функції все ще можуть з'являтися, але вимагають призначення ліцензії для роботи.  

**Ліцензія не оновлюється для користувача**  

Іноді користувачеві призначається ліцензія, але до цих пір не вдається отримати доступ до Yammer. Затримки частіше виникають під час виконання завдання масового ліцензування. Користувачі Yammer можуть не оновлюватись в тому самому порядку, що й ліцензії змінюються в Azure AD, оскільки система працює асинхронно. Зачекайте до 24 годин, перш ніж відкрити справу підтримки, щоб повідомити про проблеми з синхронізацією ліцензій.  

**Масове призначення ліцензії**  

Ліцензії можна призначити через центр адміністрування або сценаріїв PowerShell. Щоб отримати додаткові відомості див. [призначте ліцензії користувачам](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) і [призначте ліцензії для облікових записів користувачів за допомогою Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Служба підтримки Microsoft не надає допомоги у створенні сценаріїв, але документація на призначення ліцензії Yammer доступна. Для отримання додаткових відомостей див. [керування ліцензіями Yammer за допомогою оболонки Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).