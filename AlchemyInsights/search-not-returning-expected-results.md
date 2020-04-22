---
title: 1491-пошук-не-повернення-очікується-результати
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709248"
---
# <a name="content-search-not-returning-expected-results"></a>Пошук вмісту, не повертаються очікуваних результатів

Під час запуску пошуку вмісту з Microsoft 365 безпеки & центру підтримки, може з'явитися неочікувані результати пошуку. Розглянемо наступні речі, які можуть вплинути на результати пошуку:

- **Розташування вмісту та умови пошуку**: переконайтеся, що вибрано правильне розташування вмісту та умови пошуку. Якщо ви запустили великий Пошук (з багатьма розташуваннями), розглянемо розділення його на кілька пошуків.

- **Частково індексовані елементи**: [частково індексовані елементи](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) з поштових скриньок включаються до прогнозованого результату пошуку. Проте частково індексовані елементи з сайтів у SharePoint і OneDrive не включаються в оцінку пошуку.

- **Помилки пошуку**: під час пошуку великої кількості поштових скриньок (понад 100 000 поштових скриньок), ви можете отримати помилки пошуку, з кодами помилок, ТАКИМИ як CS008-009 і CS012-002). У такому разі повторіть пошук лише для місць, де не вдалося знайти вміст. Докладнішу інформацію наведено в [цій статті](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) .
