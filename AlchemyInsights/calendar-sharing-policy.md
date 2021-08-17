---
title: Політика спільного доступу до календаря (618)
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091630"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Помилка політики під час надання спільного доступу до календаря

1. Виконайте одну з наведених нижче дій відповідно до своїх ситуацій.
    - Підключення щоб Exchange Online за допомогою Remote PowerShell. Докладні відомості див. в [Підключення використання Exchange Online Remote PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - На локальному сервері відкрийте оболонку керування Exchange керування.
2. Визначте політику спільного доступу, призначену користувачу. Для цього виконайте таку команду та зверніть увагу на повернуту політику:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Оновіть політику спільного доступу для користувача. Щоб зробити це, виконайте такі дії.
    - Відкрийте Exchange адміністрування.
    - Клацніть **Організація**, а потім двічі клацніть політику, призначену користувачу в розділі **Окремий спільний доступ.** Це політика, повернуту на кроці 2.
    - На сторінці "Правило спільного доступу" виберіть рівень спільного доступу до календаря, який потрібно дозволити в розділі Укажіть відомості, до яких **потрібно надати спільний доступ.** натисніть **кнопку Зберегти**.

Докладні відомості див. в розділі Помилка "Політика не дозволяє надавати дозволи на цьому рівні одному або крізь одержувачів", коли користувач намагається надати спільний доступ [до календаря.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
