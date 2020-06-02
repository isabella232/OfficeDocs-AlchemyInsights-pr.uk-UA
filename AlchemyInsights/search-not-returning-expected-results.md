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
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510593"
---
# <a name="content-search-not-returning-expected-results"></a>Пошук вмісту, не повертаються очікуваних результатів

Під час запуску пошуку вмісту з Microsoft 365 безпеки & центру підтримки, може з'явитися неочікувані результати пошуку. Розглянемо наступні речі, які можуть вплинути на результати пошуку:

- **Розташування вмісту та умови пошуку**: переконайтеся, що вибрано правильне розташування вмісту та умови пошуку. Якщо ви запустили великий Пошук (з багатьма розташуваннями), розглянемо розділення його на кілька пошуків.

- **Частково індексовані елементи**: [частково індексовані елементи](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) з поштових скриньок включаються до прогнозованого результату пошуку. Проте частково індексовані елементи з сайтів у SharePoint і OneDrive не включаються в оцінку пошуку.

- **Помилки пошуку**: під час пошуку великої кількості поштових скриньок (понад 100 000 поштових скриньок), ви можете отримати помилки пошуку, з кодами помилок, ТАКИМИ як CS008-009 і CS012-002). У такому разі повторіть пошук лише для місць, де не вдалося знайти вміст. Докладнішу інформацію наведено в [цій статті](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
