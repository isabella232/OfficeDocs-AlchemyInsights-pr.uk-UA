---
title: Виправлення параметрів політики та поштової скриньки користувача
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695897"
---
# <a name="fix-user-policymailbox-settings"></a>Виправлення параметрів політики та поштової скриньки користувача

Це повідомлення вплине на настройки небажаної пошти в поштовій скриньці. Щоб переглянути настройки, виконайте наведені нижче дії.

1. Запуск оболонки керування Exchange. Докладні відомості наведено в статті [відкриття оболонки керування Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Виконати цю команду (за допомогою адреси електронної пошти користувача):  **Get-mailboxjunkmailconfiguration-Identity "User@domain.com"**
3. Перевірте, чи є адреса електронної пошти відправника, що входить до складу **Trusedsendersanddomains** або **blockkedsendersanddomains**. Якщо адреса електронної пошти міститься в одному з списків, можливо, доведеться видалити його. Докладні відомості можна знайти в статті " [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)".
