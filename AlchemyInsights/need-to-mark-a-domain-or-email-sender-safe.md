---
title: Потрібно позначити домен або відправника електронної пошти як надійний?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792153"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Потрібно позначити домен або відправника електронної пошти як надійний?

- Ми не **рекомендуємо** використовувати списки надійних відправників, оскільки він відкриває організацію для спаму, фішингових і спуфінгових атак.
- Проте якщо вимоги компанії висувають певні вимоги, для цього радимо **[використовувати](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** правила потоків пошти.  Наші указівки гарантують, що автентифікація відправника (перевіряє, що домен надсилання не спуфінгується). **Примітка.** Ми не радимо виправляти хибні результати за допомогою списків надійних відправників, оскільки винятки з фільтрування спаму можуть відкрити організацію в атаках безпеки. Якщо ваші користувачів отримують повідомлення, помічені як спам або небажана пошта, повідомте про повідомлення та файли до **[корпорації Майкрософт.](https://protection.office.com/reportsubmission)**
- Надійні відправники в Outlook, список дозволених відправників або  список дозволених доменів у політиках захисту від спаму слід уникати, оскільки відправники не можуть обійти всі спам, спуфінг і фіш-захист і автентифікацію відправника (SPF, DKIM, DMARC). Цей метод краще використовувати лише для тимчасового тестування.
