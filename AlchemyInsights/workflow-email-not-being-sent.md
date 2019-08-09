---
title: Робочий процес не надіслане
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 49c510668f4c73a71495b89ee9f810d4e7244da3
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270693"
---
# <a name="workflow-email-is-not-being-sent"></a>Робочий процес не надіслане

1. Лист від робочі процеси не надсилаються до всіх користувачів, або лише певним користувачам, або ви бачите помилку **повідомлення електронної пошти не може бути надіслано. Переконайтеся, що електронна пошта має непридатне**.

    Перевірте, якщо користувач існує у **Всіх людей** дозволи групі (списку відомостей про користувача) для цієї колекції сайтів.  Скуштуйте прямій URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Якщо користувач не існує, переконайтеся, що користувач буде підписано в сторінку. 
    - Якщо це із зовнішнім користувачем, переконайтеся, що їх запрошення було прийнято.
    - Якщо користувач дійсно існує у групі дозволи, переконайтеся, що адреса електронної пошти правильна.
    - Якщо адреси електронної пошти користувачів не тут, потім створити зразок оповіщення для цього користувача, який змушує синхронізацію цього облікового запису користувача із профілів користувачів SharePoint для цієї колекції сайтів.
 
2. Лист від робочі процеси надсилаються адміністраторам колекції сайтів, а не іншим користувачам і бачити помилки **HTTP Заборонене до <spam> <spam> ** <spam> <spam>.
 

    Подивитися [Відмовлено в доступі коли послав електронну пошту, групи](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).

    Крім того, переконайтеся, що **режим обмеженим доступом користувача дозволу lockdown** функції колекції сайтів не є активним.


## <a name="related-topics"></a>Пов’язані теми
Хочете спробувати Microsoft потік в SharePoint Online?
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і потік](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


