---
title: Піктограма календаря не відображається в клієнті Teams
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
- "9001219"
- "4375"
ms.openlocfilehash: 7881d6837cb7d99180d2cc1b28d327ce12e4b836d33e4fca099569d4f72510fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989612"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a>Піктограма календаря не відображається в клієнті Teams

Вкладці "Календар" у Teams потрібен доступ до поштової скриньки Exchange через веб-служби Exchange. Поштова скринька Exchange може бути онлайновою або локальною. Для онлайнових користувачів вкладка "Календар" не відображається. Переконайтеся, що [вони мають ліцензію на поштову скриньку Exchange Online і що поштову скриньку ввімкнуто](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).

Якщо користувач має дійсну поштову скриньку в Exchange Online, але вкладка "Календар" не відображається, можливо, виникли неполадки в мережі. Скористайтеся [засобом аналізу віддаленого доступу Microsoft Remote](https://testconnectivity.microsoft.com/) і запустіть **перевірку підключення до веб-служб Microsoft Exchange** для користувача, який зазнав впливу.

Перегляньте [програми Teams (політики налаштування програми)](https://admin.teams.microsoft.com/policies/app-setup), щоб переконатися, що програму "Календар" не вилучено з політики, яка застосовується до користувача (зазвичай **із глобальної політики, яка використовується за замовчуванням для всієї організації**).

Якщо ваші користувачі перебувають у локальному середовищі, переконайтеся, що гібридна конфігурація справна. Щоб вирішити проблему, скористайтеся [майстром гібридної конфігурації](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).

Зверніть увагу, що [для Teams необхідно інсталювати Exchange 2016 CU3 або новішої версії](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).
