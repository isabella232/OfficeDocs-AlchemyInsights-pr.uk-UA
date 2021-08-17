---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052731"
---
# <a name="content-search-not-returning-expected-results"></a>Пошук вмісту не повертає очікувані результати

Коли пошук вмісту виконується в Центрі Microsoft 365 безпеки &, результати пошуку можуть з'явитися неочікувані. Розглянемо такі речі, які можуть вплинути на результати пошуку:

- **Розташування вмісту та умови пошуку.** Переконайтеся, що ви вибрали правильні розташування вмісту та умови пошуку. Якщо шукано велике значення (з багатьма розташуваннями), спробуйте розділити його на кілька пошукових запитів.

- **Частково індексовані елементи:**  [частково індексовані](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) елементи з поштових скриньок включено до орієнтовних результатів пошуку. Проте частково індексовані елементи із сайтів на SharePoint і OneDrive не включено в оцінку пошуку.

- Помилки **пошуку.** Під час пошуку великої кількості поштових скриньок (понад 100 000 поштових скриньок) можуть з'явитися повідомлення про помилку пошуку з кодами помилок, наприклад CS008-009 і CS012-002. У такому разі повторіть спробу пошуку лише за розташуваннями вмісту, які не вдалося знайти. Докладні  [відомості див.](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) в цій статті.
