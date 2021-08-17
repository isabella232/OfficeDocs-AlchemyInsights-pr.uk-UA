---
title: 1332 OWA – правила для папки "Вхідні" не виконуються для поштової скриньки
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
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040923"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Правило для папки "Вхідні" працює ненавмисно

Перевірте наведені нижче параметри в інтернет-версія Outlook:

- Повідомлення можна переспрямовувати, пересилати або відполікати на них на основі правил для папки "Вхідні" лише один раз. Правило переспрямування (правило для папки "Вхідні" або правило пересилання пошти, яке також називається правилом транспортування), може додати до повідомлення щонайбагатні десять одержувачів пересилання. Докладні відомості див. в [описах обмежень правил журналів, транспортування та вхідних повідомлень.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Правила для папки "Вхідні" не працюють в додатковій поштовій скриньці протоколування. Докладні відомості про альтернативну поштову скриньку протоколювати див. в додатковій поштовій [скриньці протоколування.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Відомості про вирішення цих проблем див. [в статті бази 2829319.](https://support.microsoft.com/kb/2829319)

Якщо попередні проблеми не застосовуються, запустіть звіт діагностики правил для папки "Вхідні", перш ніж повідомити про проблему службі підтримки Microsoft.

1. Відкрийте поштову скриньку в інтернет-версія Outlook натисніть кнопку <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Настройки**  >  **Переглянути всі Outlook Настройки**  >  **Пошта**  >  **Правила**.

2. У нижній частині сторінки клацніть посилання Якщо ваші правила не працюють, клацніть тут, щоб створити **звіт діагностики.**
