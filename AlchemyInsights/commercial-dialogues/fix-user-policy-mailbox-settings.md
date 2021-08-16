---
title: Виправлення настройок політики користувача або поштової скриньки
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
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034739"
---
# <a name="fix-user-policymailbox-settings"></a>Виправлення настройок політики користувача або поштової скриньки

Параметри небажаної пошти в поштовій скриньці, на які це вплинуло повідомлення. Щоб переглянути параметри, виконайте такі дії:

1. Запустіть Exchange Керування. Докладні відомості [див. в сторінці Відкриття оболонки Exchange керування.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Виконайте цю команду (за допомогою адреси електронної пошти користувача):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Перевірте, чи є адреса електронної пошти відправника частиною **trustedSendersAndDomains** або **BlockedSendersAndDomains.** Якщо адреса електронної пошти міститься в одному зі списків, можливо, її доведеться видалити. Докладні відомості див. в статтях Настроювання параметрів поштової [скринькиJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
