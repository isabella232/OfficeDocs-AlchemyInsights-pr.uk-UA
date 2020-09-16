---
title: Повідомлення електронної пошти робочого циклу не надсилатиметься
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
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749030"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>Повідомлення електронної пошти робочого циклу не надсилатиметься для списку або бібліотеки SharePoint

1. Повідомлення електронної пошти з робочих циклів не надсилатимуться всім користувачам або лише певним користувачам, або відображається повідомлення про помилку, **яке не можна надіслати. Переконайтеся, що в повідомленні електронної пошти є дійсний одержувач**.

    Перевірте, чи є користувач у групі дозволи " **усі користувачі** " (список відомостей про користувачів) для цієї колекції сайтів.  Зразок прямої URL-адреси: https:// <tenant> . SharePoint.com/Sites/ <sitename> /_layouts/15/Peopl.aspx? Membershippid = 0

    - Якщо користувач не існує, переконайтеся, що користувач ввійшов до сторінки. 
    - Якщо це зовнішній користувач, переконайтеся, що їх запрошення прийнято.
    - Якщо користувач існує у групі дозволи, переконайтеся, що адреса електронної пошти правильна.
    - Якщо адресу електронної пошти користувачів не настроєно, а потім створіть зразок оповіщення для цього користувача, який примусово синхронізує цей обліковий запис користувача від профілів користувачів SharePoint до цієї колекції сайтів.
 
2. Електронна пошта від робочих циклів надсилатиметься адміністраторам колекції сайтів, але не до інших користувачів і не бачить помилку **http, забороненої <span>https:</span>//url/_vti_bin/Client.xvc.SP.utilities.Utility.sendemail**.
 

    Переглянути [відмовлено в доступі під час надсилання повідомлення електронної пошти групі SharePoint](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).

    Крім того, переконайтеся, що функція " **режим блокування дозволів користувачів із обмеженим доступом** " не активна.


## <a name="related-topics"></a>Пов’язані теми
Хочете спробувати Microsoft Flow у службі SharePoint Online?
- [Створення потоку](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint і передавання](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


