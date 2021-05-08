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
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286701"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Потрібно позначити домен або відправника електронної пошти як надійний?

- Ми не **рекомендуємо** використовувати списки надійних відправників, оскільки він відкриває організацію для спаму, фішингових і спуфінгових атак.
- Проте за наявності бізнес-вимог рекомендуємо для цього **[використовувати Flow пошти.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**  Наші указівки гарантують, що автентифікація відправника (перевіряє, що домен надсилання не спуфінгується). **Примітка.** Ми не радимо виправляти хибні результати за допомогою списків надійних відправників, оскільки винятки з фільтрування спаму можуть відкрити організацію в атаках безпеки. Якщо ваші користувачів отримують повідомлення, помічені як спам або небажана пошта, повідомте про повідомлення та файли до **[корпорації Майкрософт.](https://protection.office.com/reportsubmission)**
- Сейф Відправників зі списків Outlook, дозволених відправників або дозволених доменів у політиках захисту від спаму слід уникати, оскільки відправники не можуть обійти весь спам, спуфінг і фіш-захист і автентифікацію відправника (SPF, DKIM, DMARC).  Цей метод краще використовувати лише для тимчасового тестування.
- Щоб перевірити, чи не обійти певне повідомлення електронної пошти для перевірки антиспамового аналізу, установіть прапорець "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), див. в розділі Заголовки антиспамового **[повідомлення.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Оскільки корпорація Майкрософт хоче за замовчуванням захистити наших [клієнтів,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)деякі заміни клієнтів не застосовуються до зловмисних програм і високоякісного фішингу. До цих перевизначень належать: o Allowed sender lists or allowed domain lists (anti-spam policies) o Outlook Сейф o IP Allow List (фільтрація підключень) 
- Єдине перевизначає, що дає змогу фішингові повідомлення з високою довірчістю обходити фільтрування Exchange правила пересилання пошти (також відомі як правила транспортування). Відомості про те, як обійти фільтрування за допомогою правил потоку пошти, див. в цій **[статтях.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**