---
title: Піктограма календаря не відображається в Microsoft Teams клієнта
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: edd6b4a2d94b03cf4ae7bf3a8d6332ed94a7e8263aba9df1f9588eecbd0ce05a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54120025"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a>Піктограма календаря не відображається в Microsoft Teams клієнта

**Вкладка** календаря в Teams вимагає доступу до поштової скриньки Exchange за допомогою Exchange-служб. Поштова Exchange може бути онлайн або локально. Якщо користувачі в Інтернеті не бачать вкладку **Календар,** переконайтеся, що їм ліцензовано ліцензію Exchange Online поштовій скриньці, а [поштову скриньку активовано](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes). Якщо користувачі є локальними, потрібно переконатися, що гібридна конфігурація справна. Щоб вирішити проблему, скористайтеся [майстром гібридної конфігурації](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent). Зверніть увагу, що [для Teams необхідно інсталювати Exchange 2016 CU3 або новішої версії](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).

Докладні відомості та вказівки з виправлення неполадок див. [в Microsoft Teams та Exchange Server взаємодії.](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)
