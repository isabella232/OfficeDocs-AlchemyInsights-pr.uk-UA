---
title: Політика спільного доступу до календаря 618
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684251"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Помилка політики під час надання спільного доступу до календаря

1. Виконайте одну з наведених нижче дій відповідно до ситуації.
    - Підключіться до служби Exchange Online за допомогою віддаленого PowerShell. Додаткові відомості наведено в статті [підключення до служби Exchange Online за допомогою віддаленого PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - На локальному сервері відкрийте оболонку керування Exchange.
2. Визначте політику спільного доступу, призначену користувачу. Щоб виконати цю дію, виконайте таку команду та зверніть увагу на те, що політика повернулась:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Оновіть політику спільного доступу для користувача. Щоб зробити це, виконайте такі дії.
    - Відкрийте Центр адміністрування Exchange.
    - Виберіть елемент **організація**, а потім двічі клацніть політику, призначену користувачу під **окремим спільним доступом**. Це політика, повернуте на кроці 2.
    - На сторінці правило спільного доступу виберіть рівень спільного доступу до календаря, який потрібно дозволити в розділі **Укажіть відомості, які потрібно надати спільний доступ**. натисніть кнопку **зберегти**.

Для отримання додаткових відомостей див.: ["політика не дає дозволу на надання дозволів на цей рівень до одного або кількох одержувачів" під час спроби користувача надати спільний доступ до календаря](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
