---
title: Виправлення неполадок, пов'язаних із подіями з електронної пошти
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
- "9000301"
- "5765"
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105373"
---
# <a name="troubleshooting-events-from-email"></a>Виправлення неполадок, пов'язаних із подіями з електронної пошти

1. Перевірка активації функції для поштової скриньки: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Потім перегляньте журнали "Події з електронної пошти" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. У журналах "Події з електронної пошти" знайдіть елемент InternetMessageId, який збігається з елементом у поштовій скриньці.  

4. Параметр TrustScore визначає, чи додається елемент. Події додаються, лише якщо значення TrustScore = "Trusted" (Довіряти).

Значення TrustScore визначається властивостями SPF, Dkim або Dmarc у заголовку повідомлення.

Щоб переглянути ці властивості, виконайте наведені нижче дії.

**Класичний Outlook**

- Відкриття елемента
- File -> Properties -> Internet Headers

або

**MFCMapi**

- Перехід до елемента в папці "Вхідні"
- Знайдіть PR_TRANSPORT_MESSAGE_HEADERS_W

Ці властивості визначаються та записуються під час транспортування та маршрутизації. Щоб додатково виправити неполадки, може знадобитися виконати вказівки зі служби підтримки транспортування, пов'язаної з помилками SPF, DKIM і DMARC.