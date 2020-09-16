---
title: 1491 – пошук-не – повернення – очікувані результати
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740495"
---
# <a name="content-search-not-returning-expected-results"></a>Пошук вмісту не повертає очікувані результати

Під час виконання пошуків вмісту з центру відповідності & безпеки Microsoft 365 може з'явитися несподівані результати пошуку. Зверніть увагу на наведені нижче дії, які можуть вплинути на результати пошуку.

- **Розташування вмісту та умови пошуку**: переконайтеся, що вибрано відповідні розташування вмісту та умови пошуку. Якщо ви запускали великий Пошук (з багатьма розташуваннями), спробуйте розділити її на кілька пошуків.

- **Частково індексовані об'єкти**:  [частково індексовані об'єкти](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) з поштових скриньок включаються до оціночних результатів пошуку. Проте частково індексовані об'єкти з сайтів у службі SharePoint і OneDrive не включаються в оціночну оцінку.

- Помилки **пошуку**: під час пошуку великої кількості поштових скриньок (понад 100 000 поштових скриньок) ви можете отримати повідомлення про помилку пошуку з кодами помилок, наприклад CS008-009 і CS012-002). У цьому випадку повторіть пошук лише для невиконаних розташувань вмісту. Перегляньте  [цю статтю](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) , щоб отримати докладніші відомості.
