---
title: Не вдається надіслати й отримати повідомлення електронної пошти на адресу Office 365 через вимкнення протоколів TLS 1.0 і TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054927"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Не вдається надіслати й отримати повідомлення електронної пошти на адресу Office 365 через вимкнення протоколів TLS 1.0 і TLS 1.1

Як підтверджено в Центрі повідомлень після вилучення повідомлень MC229914, TLS 1.0 і TLS 1.1, припинення підтримки почалося забезпечення Exchange Online кінцевих точок потоку пошти. Незабаром Office 365 більше не прийматиме підключення електронної пошти TLS 1.0 і TLS 1.1 із зовнішніх джерел. Крім того, Exchange Online не використовуватиме для надсилання вихідної електронної пошти TLS 1.0 або 1.1. Якщо ви стикаєтеся з проблемами через вимкнення протоколу TLS 1.0 або 1.1, може виникнути одна з таких помилок:

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Помилка в перегляді черги локального сервера, який надсилає повідомлення електронної пошти до Officer 365- розгорнуто підключення 421 4.4.2 через SocketError
- Помилка в журналі протоколу надсилання з'єднувача на сервері, який надсилає електронну пошту Office 365- узгодження TLS з помилкою SocketError [](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)
- Помилка в журналі протоколу надсилання або отримання з'єднувача – '451 5.7.3 Must issue a STARTTLS command first'

Якщо у вас виникли будь-які з наведених вище помилок, переконайтеся, що на сервері, який надсилає або отримує електронну пошту, активовано протокол TLS 1.2, перевіривши наведені нижче розділи реєстру.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001 [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS** 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Якщо ви вносите будь-які зміни в наведених вище розділах реєстру, щоб активувати TLS 1.2, перезапустіть сервер, щоб зміни набрали сили. Також переконайтеся, що у вас інстальовано найновіші Windows Exchange оновлення.

Докладні відомості:

- [Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 – спільнота Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Довідник із TLS 2. Увімкнення TLS 1.2 та виявлення клієнтів, які не використовують цю програму, – спільнота Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Докладні відомості про сценарії електронної пошти, якщо версії TLS не можна узгодити з Exchange Online – спільнота Microsoft Tech](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
