---
title: Електронна пошта робочого циклу не надсилаються
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766154"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Електронна пошта робочого циклу не надсилається до списку або бібліотеки SharePoint

1. Повідомлення електронної пошти з робочих циклів не надсилаються всім користувачам або лише певним користувачам, або відображається повідомлення про помилку, **яке не вдалося надіслати. Переконайтеся, що повідомлення електронної пошти має дійсний одержувач**.

    Перевірте, чи існує користувач у групі дозволи **всіх** користувачів (список відомостей про користувача) для цієї колекції сайтів.  Приклад прямої URL-адреси<tenant>: https://<sitename>. SharePoint.com/Sites//_layouts/15/Car.GRA? Членпідкод = 0

    - Якщо користувач не існує, переконайтеся, що користувач увійшов до сторінки. 
    - Якщо це зовнішній користувач, переконайтеся, що їхнє запрошення прийняте.
    - Якщо користувач існує у групі дозволів, переконайтеся, що адреса електронної пошти правильна.
    - Якщо тут не встановлено адресу електронної пошти користувачів, створіть зразок оповіщення для цього користувача, який примушує синхронізацію цього облікового запису користувача з профілів користувачів SharePoint до цієї колекції сайтів.
 
2. Повідомлення електронної пошти з робочих циклів надсилаються адміністраторам колекції сайтів, але не іншим користувачам і відображається повідомлення про помилку **http заборонено <span>https:</span>//URL/_vti_bin/Client.xvc.SP.utilities.Utility.sendemail**.
 

    Переглянути [відмовлено в доступі під час надсилання повідомлення електронної пошти до групи SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Крім того, переконайтеся, що функція **доступу до прав користувачів із обмеженим доступом до режиму блокування** сайтів не активна.


## <a name="related-topics"></a>Пов’язані теми
Бажаєте спробувати Microsoft Flow у SharePoint Online?
- [Створити потік](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


