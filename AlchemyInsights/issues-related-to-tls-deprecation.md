---
title: Не вдається надіслати або отримати повідомлення електронної пошти з Office 365 через протокол TLS 1,0 і TLS 1,1 інвалідності
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747112"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Не вдається надіслати або отримати повідомлення електронної пошти з Office 365 через протокол TLS 1,0 і TLS 1,1 інвалідності

Як підтвердив повідомлення центру повідомлень MC229914, TLS 1,0 і TLS 1,1, Початок виконання для кінцевих точок потоку пошти Exchange Online. Незабаром Office 365 більше не прийматиме протокол TLS 1,0 і TLS 1,1 підключення до електронної пошти із зовнішніх джерел. Крім того, Exchange Online ніколи не використовуватиме протокол TLS 1,0 або 1,1, щоб надсилати вихідні повідомлення електронної пошти. Якщо ви зіткнулися з проблемами через TLS 1,0 або 1,1 інвалідності, може виникнути одна з таких помилок:

- Відправник отримує звіт про недоставку назад-' 421 4.4.2 з'єднання розірвано через помилку Sokeketerror '
- Помилка в засобі перегляду черг локального сервера, на якому надсилається повідомлення електронної пошти офіцеру 365 – ' 421 4.4.2, через помилку «Сокіл»
- Помилка в журналі "Надіслати [протокол](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) з'єднувача" на сервері надсилання повідомлення електронної пошти до служби Office 365 – TLS не вдалося з помилкою Sokeketerror
- Помилка в журналі "надсилати або отримувати сполучну лінію": "451 5.7.3 має видати спочатку команду STARTTLS"

Якщо у вас виникли наведені вище помилки, переконайтеся, що сервер, який надсилає або отримує повідомлення електронної пошти, має TLS 1,2 увімкнуто, перевіривши наведені нижче розділи реєстру.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ клієнт] **"Disablebydefault" = DWORD: 00000000 "увімкнено" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Server] **"Disablebydefault" = DWORD: 00000000 "увімкнено" = DWORD: 00000001**

Якщо ви вносите будь-які зміни в зазначених вище розділах реєстру, щоб увімкнути протокол TLS 1,2, перезавантажте сервер, щоб зміни набрали сили. Також переконайтеся, що інстальовано найновіші оновлення Windows і Exchange.

Докладні відомості:

- [Посібник із сервера Exchange Server, частина 1: підготовка до TLS 1,2-спільнота Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Посібник із сервера Exchange Server частина 2: ввімкнення TLS 1,2 і визначення клієнтів, які не використовують її-спільнота Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Загальні відомості про сценарії електронної пошти, якщо версії TLS не можна узгодити з спільнотою Exchange Online – Microsoft Tech спільноти](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
