---
title: Визначення дії з правилом папки "Вхідні" в контрольних журналах
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331144"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Визначення дії з правилом папки "Вхідні" в контрольних журналах

Ви можете скористатися пошуком контрольного журналу в Центр відповідності Microsoft 365, щоб переглядати події правил для папки "Вхідні" (створення, змінення та видалення правил для папки "Вхідні").

1. Виконайте одну з таких дій:
   - У розділі Центр відповідності Microsoft 365 <https://compliance.microsoft.com> перейдіть до пункту Аудит  \> **рішень.** Або, щоб перейти безпосередньо на сторінку **"Аудит",** <https://compliance.microsoft.com/auditlogsearch> скористайтеся .
   - На порталі Microsoft 365 Defender перейдіть <https://security.microsoft.com> до в меню **Audit (Аудит).** Або, щоб перейти безпосередньо на сторінку **"Аудит",** <https://security.microsoft.com/auditlogsearch> скористайтеся .

2. На вкладці **Пошук** на сторінці **Аудит налаштуйте** такі параметри:
   - **Діапазон дати й часу.** У полях  Початок і Кінець виберіть діапазон дат **і** часу.
   - **Дії.** Виберіть одне або кілька з наведених нижче значень.
     - **New-InboxRule Create inbox rule from Outlook Web App**
     - **Set-InboxRule Modify rule from Outlook Web App**.
     - **Оновлення правил для папки "Вхідні" Outlook клієнта**

3. Завершивши, натисніть кнопку **Пошук**. Дії відображаються на новій **сторінці Пошук у контрольі.**

4. Виберіть дію в результатах, щоб відкрити докладні відомості. Відомості про настройки правил для папки "Вхідні" відображаються в **полі Параметри.**

Докладні відомості див. [в описі того, чи створив користувач правило для папки "Вхідні"](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule).
