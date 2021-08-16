---
title: Електронна пошта робочого циклу не надсилається
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
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072541"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Електронна пошта робочого циклу не надсилається SharePoint списку або бібліотеки

1. Електронна пошта з робочих циклів не надсилається всім користувачам або лише певним користувачам, або відображається повідомлення про помилку Повідомлення електронної пошти не можна надіслати. Переконайтеся, що в повідомлення електронної пошти вказано припустимого **одержувача.**

    Перевірте, чи є користувач у **групі дозволів Усі** користувачі (список відомостей про користувача) для цієї колекції сайтів.  Зразок прямої URL-адреси: https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx? MembershipGroupId=0

    - Якщо користувача не існує, переконайтеся, що користувач увійшов на сторінку. 
    - Якщо це зовнішній користувач, переконайтеся, що його запрошення прийнято.
    - Якщо користувач у групі дозволів, перевірте правильність адреси електронної пошти.
    - Якщо тут не задається адреса електронної пошти користувачів, створіть зразок оповіщення для цього користувача, який змушує синхронізацію цього облікового запису користувача з профілів користувачів SharePoint із цією колекцією сайтів.
 
2. Електронна пошта з робочих циклів надсилається адміністраторам колекції сайтів, але не іншим користувачам, і відображається помилка HTTP Заборонено на **<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.
 

    Докладні [відомості див. в SharePoint Access Denied when](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)you send an email to a SharePoint(

    Також переконайтеся, що **режим блокування дозволів** користувачів з обмеженим доступом неактивний.


## <a name="related-topics"></a>Пов’язані теми
Бажаєте спробувати Microsoft Flow в SharePoint Online?
- [Створення Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


