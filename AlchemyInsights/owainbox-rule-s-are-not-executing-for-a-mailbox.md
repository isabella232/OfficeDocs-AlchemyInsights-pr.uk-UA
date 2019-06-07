---
title: 1332 OWA - вхідні правила не виконуєте для поштової скриньки
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762244"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Вхідні правило не працює належним чином

Підтвердження таких настройок:

- Можна переспрямувати повідомлення, пересиланню чи була надіслана відповідь, автоматично заснований на правилах вхідної тільки один раз. Переспрямування правило (правило для вхідних повідомлень або правило потік пошти, також відомі як правила транспортування) можна додати максимум десять пересилання одержувачам повідомлення. Докладніше перегляньте [журнал, транспорту і «вхідні» правилом меж](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Правила для папки «Вхідні» не працюють на поштову скриньку альтернативний журналів. Докладніше про поштової скриньки протоколювання альтернативний побачити [Альтернативний журнальної поштової скриньки](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Для усунення цих проблем, побачити [2829319 КБ](https://support.microsoft.com/kb/2829319).

Якщо не застосовувати попередніх випусків, запустити папки «Вхідні» правилом діагностичний звіт перед ескалації питання до служби підтримки Microsoft:

1. Відкриття поштової скриньки в Outlook в Інтернеті та кнопку **Параметри** \> **Параметри** \> **упорядкувати електронну** \> **Вхідні правила**.

2. У нижній частині сторінки натисніть, **Якщо правила не працюють натисніть тут, щоб створити діагностичний звіт**.
