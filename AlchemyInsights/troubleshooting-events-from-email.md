---
title: Виправлення неполадок із електронною поштою
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658755"
---
# <a name="troubleshooting-events-from-email"></a>Виправлення неполадок із електронною поштою

1. Перевірка функції для поштової скриньки: **Get-EventsFromEmailConfiguration-Identity <mailbox> **

2. Після цього перейдіть на вкладку "події з електронної пошти", що **експортується – MailboxDiagnosticLogs <mailbox> -компонент "хронопрофіль** "

3. У журналах "події з електронної пошти" Дізнайтеся, що відповідає елементу в поштовій скриньці.  

4. "Довірчого значення" визначає, чи додано елемент або ні. Події буде додано лише за умови, що довірчі = "надійні".

Показник Truecscore визначається за властивостями SPF, DKIM або DKIM, які знаходяться в заголовку повідомлення.

Щоб переглянути ці властивості, виконайте наведені нижче дії.

**Робочий стіл Outlook**

- Відкриття елемента
- Властивості файлу > – > заголовки Інтернету

або

**Mffmapi**

- Перехід до елемента в папці "Вхідні"
- Пошук PR_TRANSPORT_MESSAGE_HEADERS_W

Ці властивості визначаються та записуються під час транспортування та маршрутизації. Щоб отримати додаткові виправлення неполадок, можливо, знадобиться стежити за допомогою транспортної підтримки про помилки в SPF, DKIM і. або DKIM.