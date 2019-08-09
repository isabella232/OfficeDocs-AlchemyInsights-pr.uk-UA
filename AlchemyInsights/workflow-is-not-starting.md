---
title: Робочий процес не запускається
ms.author: efrene
author: efrene
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
ms.openlocfilehash: a3bac74c19a77b7703f948c1d8b6bcd182e9b075
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270801"
---
# <a name="workflow-is-not-starting"></a>Робочий процес не запускається

- SharePoint 2010 і SharePoint 2013 робочі процеси не запускається.

    - Якщо робочого процесу не запускається, можливо питання тимчасові обслуговування де користувачів можуть виникнути тимчасовим затримкам з робочого процесу прогресу. Перевірте [Службу здоров'я Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) щоб побачити, якщо ваша організація є вплив.

    - Якщо більш ніж 24 години пройшло з тих пір ви вперше побачив це питання, будь ласка, увійдіть квиток підтримки. У багатьох випадках ми вже працюємо над вирішенням. Будь ласка, надайте нам принаймні за 24 години до виконання рішення.

- SharePoint 2010 робочі процеси затримується на старті.

    - Це відбувається, якщо робочий процес спрацьовує у великих партіях. (наприклад, коли кілька елементів додаються відразу).

    - Робочі процеси не призначений для запуску в режимі реального часу, так що затримка — за дизайн поведінки.

   -  Якщо робочий процес комплекс розширюваний об'єктно розмітки мови (XMOL), компіляції може бути повільним. Перевірити [цю](https://support.microsoft.com/en-us/kb/3043697) статтю.

    - Ви повинні спростити робочого процесу або редизайн його за допомогою Microsoft SharePoint робочий процес для 2013 тип платформи.

    - Якщо робочий процес історії розрісся розмір, ви можете очистити елементи або створити новий список журналу.

        Більш детальну інформацію: [Очистити історію робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Пов’язані теми
Хочете спробувати Microsoft потік в SharePoint Online?
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і потік](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


