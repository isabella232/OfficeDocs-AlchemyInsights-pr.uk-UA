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
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319969"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Потрібно позначити домен або відправника електронної пошти як надійний?

- Ми не **рекомендуємо** використовувати списки надійних відправників, оскільки він відкриває організацію для спаму, фішингових і спуфінгових атак.
- Проте якщо вимоги компанії висувають певні вимоги, для цього **[радимо використовувати Flow](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** пошти.  Наші указівки гарантують, що автентифікація відправника (перевіряє, що домен надсилання не спуфінгується). 
    **Примітка.** Ми не радимо виправляти хибні результати за допомогою списків надійних відправників, оскільки винятки з фільтрування спаму можуть відкривати організацію в атаках безпеки. Якщо ваші користувачів неправильно позначили їх як спам або небажану пошту, повідомте про повідомлення та файли **[до корпорації Майкрософт.](https://protection.office.com/reportsubmission)**
- Сейф Відправників зі списків Outlook, дозволених відправників і дозволених  доменів у політиках захисту від спаму слід уникати, оскільки відправники не можуть обійти весь спам, спуфінг і захист від фішингу та автентифікацію відправника (SPF, DKIM, DMARC). Цей метод краще використовувати лише для тимчасового тестування.
- Щоб перевірити, чи не обійти певне повідомлення електронної пошти для перевірки антиспамового аналізу, перевірте заголовок повідомлення "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN) і перегляньте заголовки антиспамового **[повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Оскільки корпорація Майкрософт хоче за замовчуванням захистити наших [клієнтів,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)деякі заміни клієнтів не застосовуються до зловмисних програм і високоякісного фішингу. До цих перевизначень належать: o Allowed sender lists or allowed domain lists (anti-spam policies) o Outlook Сейф o IP Allow List (фільтрація підключень) 
- Єдине перевизначає, що дає змогу фішингові повідомлення з високою довірою обходити фільтрування Exchange правила пересилання пошти (також відомі як правила транспортування). Відомості про те, як обійти фільтрування за допомогою правил потоку пошти, див. в цій **[статтях.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**