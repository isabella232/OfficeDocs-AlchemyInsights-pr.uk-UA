---
title: Потрібно позначити домен або відправника електронної пошти безпечним?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281240"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Потрібно позначити домен або відправника електронної пошти безпечним?

- Використання **безпечних списків відправників не рекомендується** , оскільки вона відкриває вашу організацію для спаму, phish і спуфінгу атак.
- Однак, якщо є бізнес-вимога, ми **рекомендуємо** використовувати **[правила потоку пошти](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** для цього. Наші вказівки гарантують автентичність відправника (перевірка домену, який надсилає надсилання, не є підробною). **Примітка**: не рекомендовано керувати помилковими спрацьовувань за допомогою списків надійних відправників, оскільки винятки з фільтрації спаму можуть відкрити організацію для атак безпеки. Якщо користувач (и) отримує повідомлення помилково позначено як спам або Небажана пошта, будь ласка, **[повідомляйте про повідомлення та файли до корпорації Майкрософт](https://protection.office.com/reportsubmission)**.
- Надійні відправники в Outlook, дозволені список відправників або дозволений список доменів у політиці проти спаму **слід уникати** , оскільки відправники оминають всі спам, пародія і phish Protection та автентифікацію ВІДПРАВНИКА (SPF, DKIM, DKIM). Цей метод найкраще використовувати тільки для тимчасового тестування.
