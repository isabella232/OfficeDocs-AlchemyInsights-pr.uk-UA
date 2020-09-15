---
title: 1332 OWA-вхідні не виконують правила для поштової скриньки
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
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721612"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Правило для папки "Вхідні" не працює належним чином

Перевірте наведені нижче настройки в Інтернет-версії Outlook.

- Повідомлення можна перенаправлятися, пересилати або відповідати автоматично на основі правил для папки "Вхідні" лише один раз. Правило переспрямування (правило для папки "Вхідні" або "потік пошти", також відомий як правило транспортування) може додавати до повідомлення максимум десяти одержувачів пересилання. Докладні відомості наведено в статті [обмеження правил для журналу, транспорту та папки "Вхідні"](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Правила для папки "Вхідні" не працюють в альтернативному поштовій скриньці журналювання. Докладні відомості про альтернативну поштову скриньку журналювання наведено в статті [Альтернативна поштова скринька журналів](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Щоб вирішити ці проблеми, ознайомтеся з пунктом [KB 2829319](https://support.microsoft.com/kb/2829319).

Якщо попередні проблеми не застосовуватимуться, запустіть звіт про діагностику правил для папки "Вхідні", перш ніж перерости цю проблему до служби підтримки Microsoft.

1. Відкрийте поштову скриньку в Інтернет-версії Outlook і натисніть кнопку <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Параметри**  >  **Переглянути всі настройки Outlook**  >  **Пошта**  >  **Правила**.

2. У нижній частині сторінки клацніть, **Якщо правила не працюють, натисніть тут, щоб створити діагностичний звіт**.
