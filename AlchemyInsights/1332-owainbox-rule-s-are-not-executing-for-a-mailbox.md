---
title: 1332 OWA - вхідні правила не виконуєте для поштової скриньки
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28319636"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Вхідні правило не працює належним чином

Підтвердження таких настройок:
  
- Можна переспрямувати повідомлення, пересиланню чи була надіслана відповідь, автоматично заснований на правилах вхідної тільки один раз. Переспрямування правило (правило для вхідних повідомлень або правило потік пошти, також відомі як правила транспортування) можна додати максимум десять пересилання одержувачам повідомлення. Докладніше перегляньте [журнал, транспорту і «вхідні» правилом меж](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Правила для папки «Вхідні» не працюють на поштову скриньку альтернативний журналів. Докладніше про поштової скриньки протоколювання альтернативний побачити [Альтернативний журнальної поштової скриньки](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Для усунення цих проблем, побачити [2829319 КБ](https://support.microsoft.com/kb/2829319).
  
Якщо не застосовувати попередніх випусків, запустити папки «Вхідні» правилом діагностичний звіт перед ескалації питання до служби підтримки Microsoft:
  
1. Відкриття поштової скриньки в Outlook в Інтернеті та кнопку **Параметри** \> **Параметри** \> **упорядкувати електронну** \> **Вхідні правила**.
    
2. У нижній частині сторінки натисніть, **Якщо правила не працюють натисніть тут, щоб створити діагностичний звіт**.
    

