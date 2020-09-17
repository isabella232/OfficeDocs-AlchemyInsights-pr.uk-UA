---
title: Запуск робочого циклу не починається
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794788"
---
# <a name="workflow-is-not-starting"></a>Запуск робочого циклу не починається

- Робочі цикли SharePoint 2010 і SharePoint 2013 не починаються.

    - Якщо робочий цикл не запускається, може виникнути тимчасова проблема служби, у якій користувачі можуть виникати періодичні затримки з прогресом робочого циклу. Перевірте [приладну дошку справності служби](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб дізнатися, чи впливає ваша організація.

    - Якщо ви вперше побачили цю проблему понад 24 години, увійдіть у службу підтримки. У багатьох випадках ми вже працюємо над вирішенням проблеми. Щоб завершити вирішення, надайте нам принаймні 24 години.

- Робочі цикли SharePoint 2010, затримані під час запуску.

    - Це трапляється, якщо робочий цикл запущено у великих партіях. (наприклад, коли кілька одиниць додаються одночасно).

    - Робочі цикли не призначені для запуску в реальному часі, тому відповідну поведінку можна виконувати в режимі конструктора.

   -  Якщо робочий цикл – це складна розширювана мова розмітки об'єктів (XMOL), то компіляцію може бути повільним. Установіть прапорець у [цій](https://support.microsoft.com//kb/3043697) статті.

    - Ви повинні спростити робочий цикл або редизайн його за допомогою типу платформи робочого циклу Microsoft SharePoint 2013.

    - Якщо журнал робочого циклу виріс великий, можливо, потрібно буде очистити елементи або створити новий список журналу.

        Додаткові відомості: [очищення журналу робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Пов’язані теми
Хочете спробувати Microsoft Flow у службі SharePoint Online?
- [Створення потоку](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і передавання](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


