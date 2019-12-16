---
title: Робочий цикл не починається
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049358"
---
# <a name="workflow-is-not-starting"></a>Робочий цикл не починається

- SharePoint 2010 і SharePoint 2013 робочі цикли не починаються.

    - Якщо робочий процес не починається, може виникнути проблема тимчасового обслуговування, коли користувачі можуть виникати періодичні затримки з прогресом робочого циклу. Перегляньте [приладну дошку стану служби](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб дізнатися, чи впливає ваша організація.

    - Якщо Минуло більше 24 годин з тих пір, як ви вперше побачили цю проблему, будь ласка, увійдіть квиток підтримки. У багатьох випадках ми вже працюємо над вирішенням. Будь ласка, дайте нам принаймні 24 годин, щоб завершити рішення.

- SharePoint 2010 робочі цикли, затримуються на початковому запуску.

    - Це відбувається, якщо робочий цикл запускається великими партіями. (наприклад, коли кілька елементів додаються одночасно).

    - Робочі цикли не призначені для запуску в режимі реального часу, тому затримка є за-дизайн поведінки.

   -  Якщо робочий процес складний, розширювана об'єкт розмітки мови (XMOL), компіляції може бути повільним. Перевірити [цю](https://support.microsoft.com//kb/3043697) статтю.

    - Ви повинні спростити робочий цикл або переробити його за допомогою типу платформи робочого циклу Microsoft SharePoint 2013.

    - Якщо історія робочого циклу зросла, можливо, потрібно видалити елементи або створити новий список журналу.

        Додаткові відомості: [очищення журналу робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Пов’язані теми
Бажаєте спробувати Microsoft Flow у SharePoint Online?
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


