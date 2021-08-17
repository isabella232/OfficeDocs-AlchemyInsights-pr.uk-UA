---
title: Пошук подій, які виконуються з правилами для папки "Вхідні"
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 626bd7515270f03e1560a3ed637e7bc60b374c5525527205d5f6775e4758f07a
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57882656"
---
# <a name="find-events-performed-on-inbox-rules"></a>Пошук подій, які виконуються з правилами для папки "Вхідні"

Коли правила для папки "Вхідні" створюють, змінюються та видаляються, події записуються в контрольний журнал. Ось як їх переглянути.

1. Виконайте одну з таких дій:
   - У розділі Центр відповідності Microsoft 365 <https://compliance.microsoft.com> перейдіть до пункту Аудит  \> **рішень.** Або, щоб перейти безпосередньо на сторінку **"Аудит",** <https://compliance.microsoft.com/auditlogsearch> скористайтеся .
   - На порталі Microsoft 365 Defender виберіть <https://security.microsoft.com> аудит .  Або, щоб перейти безпосередньо на сторінку **"Аудит",** <https://security.microsoft.com/auditlogsearch> скористайтеся .

    > [!NOTE]
    > Якщо з'явилось повідомлення про те, що потрібно ввімкнути аудит, увімкніть його зараз. Якщо цю функцію вимкнуто, результати пошуку не зможуть отримувати дані з попередніх дат.

2. На вкладці **Пошук** на сторінці **Аудит налаштуйте** такі параметри:
   - **Діапазон дати й часу.** У полях  Початок і Кінець виберіть діапазон дат **і** часу.
   - **Дії.** Виберіть **Нове правило для папки "Вхідні",** створене за Outlook Web App

3. Завершивши, натисніть кнопку **Пошук**. Дії відображаються на новій **сторінці Пошук у контрольі.**

4. Виберіть дію в результатах, щоб відкрити докладні відомості. У розділі **Параметри** можна переглянути ім'я правила, набору умов і дій, які виконуватиме правило.

Докладні відомості див. в [статтях Пошук у контрольому журналі, щоб дізнатися про поширені проблеми з підтримкою.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
