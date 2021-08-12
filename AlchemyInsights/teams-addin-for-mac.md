---
title: Teams надбудови для Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940696"
---
# <a name="teams-add-in-for-mac"></a>Teams надбудови для Mac

Щоб усунути відсутніх Teams користувачів операційної системи для Mac, виконайте такі дії:

**Крок 1.** Якщо використовується гібридне середовище Exchange локальний (2016 CU3 або пізнішої версії), скористайтеся засобом Test-HMA.ps1, щоб переконатися, що гібридну сучасну автентифікацію настроєно правильно. Докладні відомості див. в [розділ Перевірка налаштування гібридної сучасної автентифікації Outlook для iOS і Android.](https://aka.ms/TestHMAEAS)  

**Примітка** Використовуйте формат адреси UPN [(наприклад,](mailto:username@contoso.com)"username@contoso.com"), а не домен\ім'я_користувача. Зробіть це навіть для користувачів із Exchange Online поштових скриньок.

**Крок 2.** Користувач може перейти до меню **Інструменти Облікові**  >  **записи**... у Outlook для Mac, знайдіть і виберіть обліковий запис. Переконайтеся, що ім'я користувача зазначено у форматі UPN (наприклад, [username@contoso.com).](mailto:username@contoso.com)

**Крок 3.** Переконайтеся, що користувач має ліцензію Microsoft Teams користувача. Користувач має використовувати передплату на Office 365 для Mac версії 16.24 або пізнішої.