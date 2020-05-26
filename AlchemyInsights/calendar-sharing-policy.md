---
title: 618 політика спільного доступу до календаря
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373020"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Політика помилка під час спільного доступу до календаря

1. Виконайте одну з наведених нижче дій відповідно до ситуації.
    - Підключення до Exchange Online за допомогою віддаленого PowerShell. Для отримання додаткових відомостей див. [підключення до Exchange Online за допомогою віддаленого PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - На локальному сервері, відкрийте оболонку керування Exchange.
2. Визначте політику спільного доступу, призначену для користувача. Для цього виконайте таку команду та запишіть політику, що повертається:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Оновіть політику спільного доступу для користувача. Щоб зробити це, виконайте такі дії.
    - Відкрийте Центр адміністрування Exchange.
    - Клацніть **організації**, а потім двічі клацніть політику, призначену користувачу під **окремим спільним доступом**. Це політика, яка була повернена на кроці 2.
    - На сторінці правила спільного доступу виберіть рівень спільного доступу до календаря, який потрібно дозволити у розділі **Укажіть відомості, які потрібно надати спільний доступ**; натисніть кнопку **зберегти**.

Щоб отримати додаткові відомості див.: ["політика не дозволяє надання дозволів на цьому рівні один або кілька одержувачів (ів)" помилка, коли користувач намагається надати спільний доступ до календаря](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
