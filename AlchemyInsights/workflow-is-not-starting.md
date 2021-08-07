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
ms.openlocfilehash: 77a3c022a9a3a82041b4a4a70c72c2e0940c0fba27f296f07881e3abebf1e464
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53907759"
---
# <a name="workflow-is-not-starting"></a>Робочий цикл не запускається

- SharePoint 2010 і SharePoint 2013 не запускаються.

    - Якщо робочий цикл не запускається, можуть виникати тимчасові проблеми зі службою, у яких користувачі можуть час відкладати затримки перебігу робочого циклу. Перегляньте [приладну дошку справності](https://admin.microsoft.com/AdminPortal/Home/servicehealth) служб, щоб дізнатися, чи це впливає на вашу організацію.

    - Якщо з моменту виникнення цієї проблеми минає понад 24 години, надішлюйте запит на підтримку. У багатьох випадках ми вже працюємо над вирішенням цієї проблеми. Дайте нам принаймні 24 години, щоб завершити вирішення.

- SharePoint 2010 робочих циклів, які затримуються під час запуску.

    - Це трапляється, якщо робочий цикл запускається великими пакетами. (Наприклад, якщо одночасно додається кілька елементів).

    - Робочі цикли не запускаються в реальному часі, тому затримка передбачає певну поведінку.

   -  Якщо робочий цикл – це складна мова розмітки об'єкта (XMOL), компіляція може сповільнюватися. Перегляньте [цю](https://support.microsoft.com//kb/3043697) статтю.

    - Слід спростити робочий цикл або перепростити його за допомогою типу платформи робочих SharePoint Microsoft SharePoint 2013.

    - Якщо журнал робочого циклу збільшується, можливо, ви захочете видалити елементи або створити новий список журналу.

        Докладні відомості: [Видалити журнал робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Пов’язані теми
Бажаєте спробувати Microsoft Flow в SharePoint Online?
- [Створення Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
