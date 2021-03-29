---
title: Робочий цикл не запускається
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403764"
---
# <a name="workflow-is-not-starting"></a>Робочий цикл не запускається

- Робочі цикли SharePoint 2010 і SharePoint 2013 не запускаються.

    - Якщо робочий цикл не запускається, можуть виникати тимчасові проблеми зі службою, у яких користувачі можуть час відкладати затримки перебігу робочого циклу. Перегляньте [приладну дошку справності](https://admin.microsoft.com/AdminPortal/Home/servicehealth) служб, щоб дізнатися, чи це впливає на вашу організацію.

    - Якщо з моменту виникнення цієї проблеми минає понад 24 години, надішлюйте запит на підтримку. У багатьох випадках ми вже працюємо над вирішенням. Дайте нам принаймні 24 години, щоб завершити вирішення.

- Робочі цикли SharePoint 2010, які затримуються під час запуску.

    - Це трапляється, якщо робочий цикл запускається великими пакетами. (Наприклад, якщо одночасно додається кілька елементів).

    - Робочі цикли не запускаються в реальному часі, тому затримка передбачає певну поведінку.

   -  Якщо робочий цикл – це складна мова розмітки об'єкта (XMOL), компіляція може сповільнюватися. Перегляньте [цю](https://support.microsoft.com//kb/3043697) статтю.

    - Слід спростити робочий цикл або перепростити його за допомогою типу платформи робочого циклу Microsoft SharePoint 2013.

    - Якщо журнал робочого циклу збільшується, можливо, ви захочете видалити елементи або створити новий список журналу.

        Докладні відомості: [Видалити журнал робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Пов’язані теми
Хочете спробувати Microsoft Flow у SharePoint Online?
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
