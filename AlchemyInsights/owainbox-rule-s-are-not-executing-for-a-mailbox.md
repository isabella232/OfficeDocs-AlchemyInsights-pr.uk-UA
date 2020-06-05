---
title: 1332 OWA-правило для папки "Вхідні" (и) не виконує для поштової скриньки
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576581"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Правило для папки "Вхідні" не працює належним чином

Перевірте наведені нижче параметри в Outlook, в Інтернеті:

- Повідомлення може бути переадресовано, переслано або долучено до нього автоматично на основі правил вхідних повідомлень лише один раз. Правило переспрямування (правило "Вхідні" або правило потоку пошти, також відоме як правило транспортування) може додати до повідомлення щонайбільше десять одержувачів пересилання. Щоб отримати додаткові відомості, перегляньте [обмеження правил журналу, транспорту та папки "Вхідні"](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Правила для папки "Вхідні", не працюють на альтернативні журналювання поштової скриньки. Щоб отримати додаткові відомості про альтернативні журналювання поштова скринька, [див.](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)

Щоб вирішити ці проблеми, див. [KB 2829319](https://support.microsoft.com/kb/2829319).

Якщо попередні проблеми не застосовуються, запустіть звіт "правило" для діагностики "Вхідні", перш ніж перехід до проблеми служби підтримки Microsoft:

1. Відкрийте поштову скриньку в Outlook, в Інтернеті та натисніть кнопку <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Налаштуваннях**  >  **Переглянути всі налаштування Outlook**  >  **Пошти**  >  **Правилами**.

2. Унизу сторінки натисніть кнопку **, якщо правила не працюють, клацніть тут, щоб створити діагностичний звіт**.
