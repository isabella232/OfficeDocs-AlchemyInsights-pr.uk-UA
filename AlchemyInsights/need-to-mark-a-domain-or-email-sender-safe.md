---
title: Потрібно, щоб можна було відмітити домен або відправника електронної пошти в безпеці?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803266"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Потрібно, щоб можна було відмітити домен або відправника електронної пошти в безпеці?

- **Не рекомендується використовувати списки надійних відправників** , оскільки вона відкриває свою організацію в спам, phish та спуфінгу.
- Однак, якщо є потреба в бізнесі, **радимо** використовувати **[правила передавання пошти](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Наше керівництво забезпечує автентифікацію відправника (перевіряє, чи не підроблений домен). **Примітка**. не радимо керувати хибними спрацьовуванням за допомогою списків надійних відправників, оскільки винятки з фільтрування спаму можуть відкрити свою організацію для атак з безпеки. Якщо ваші повідомлення неправильно позначені як спам або Небажана пошта, **[повідомте про це повідомлення та файли до корпорації Майкрософт](https://protection.office.com/reportsubmission)**.
- Надійні відправники в Outlook, дозволені список відправників або список дозволених доменів у політиці захисту від спаму **слід уникати** , тому що відправники оминають всі функції спаму, пародія та флеш-захист, а також автентифікацію ВІДПРАВНИКА (SPF, DKIM, DKIM). Цей метод можна використовувати лише для тимчасового тестування.
