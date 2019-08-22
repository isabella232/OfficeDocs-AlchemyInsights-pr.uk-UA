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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530912"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Робочий процес не надіслане для списку або бібліотеки

1. Лист від робочі процеси не надсилаються до всіх користувачів, або лише певним користувачам, або ви бачите помилку **повідомлення електронної пошти не може бути надіслано. Переконайтеся, що електронна пошта має непридатне**.

    Перевірте, якщо користувач існує у **Всіх людей** дозволи групі (списку відомостей про користувача) для цієї колекції сайтів.  Скуштуйте прямій URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0

    - Якщо користувач не існує, переконайтеся, що користувач буде підписано в сторінку. 
    - Якщо це із зовнішнім користувачем, переконайтеся, що їх запрошення було прийнято.
    - Якщо користувач дійсно існує у групі дозволи, переконайтеся, що адреса електронної пошти правильна.
    - Якщо адреси електронної пошти користувачів не тут, потім створити зразок оповіщення для цього користувача, який змушує синхронізацію цього облікового запису користувача із профілів користувачів SharePoint для цієї колекції сайтів.
 
2. Лист від робочі процеси надсилаються адміністраторам колекції сайтів, а не іншим користувачам і бачити помилки **HTTP Заборонене до <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Переглянути [Доступ заборонено під час надсилання повідомлення електронної пошти до групи SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Крім того, переконайтеся, що **режим обмеженим доступом користувача дозволу lockdown** функції колекції сайтів не є активним.


## <a name="related-topics"></a>Пов’язані теми
Хочете спробувати Microsoft потік в SharePoint Online?
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і потік](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


