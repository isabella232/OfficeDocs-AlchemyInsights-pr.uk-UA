---
title: Усунення несправностей подій з електронної пошти
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569399"
---
# <a name="troubleshooting-events-from-email"></a>Усунення несправностей подій з електронної пошти

1. Перевірте, чи ввімкнуто функцію для поштової скриньки: **Get-подія Sfromemailconfiguration-посвідчення <mailbox> **

2. Потім подивіться на "події з електронної пошти" журнали **експорт-MailboxDiagnosticLogs <mailbox> -компонент timeprofile**

3. У журналах "події з електронної пошти" знайдіть пункт Інтернетаповідомлення, яке відповідає елементу в поштовій скриньці.  

4. Довірчого оцінка визначає, чи елемент додано чи ні. Події будуть додаватися, лише якщо довірчого показника = "довірений".

Довірчого оцінки визначається SPF, DKIM або DKIM властивості, які в заголовку повідомлення.

Щоб переглянути ці властивості:

**Desktop Outlook**

- Відкрити елемент
- Файл-> властивості-> Інтернет-заголовки

Або

**MFCMapi**

- Перехід до елемента в папці «Вхідні»
- Шукайте PR_TRANSPORT_MESSAGE_HEADERS_W

Ці властивості визначаються і записуються під час транспортування та маршрутизації. Щоб отримати додаткові відомості про виправлення неполадок, можливо, потрібно буде виконати транспортні підтримки про збої в SPF, DKIM та. or DKIM.