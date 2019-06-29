---
title: 1491-Search-Not-Returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355898"
---
# <a name="content-search-not-returning-expected-results"></a>Пошук за змістом не повертаючи очікувані результати

Під час пошуків вмісту з Office 365 безпеки & центрі дотримання, може з'явитися несподіваних результатів. Розглянути наступні речі, які можуть вплинути на результати пошуку:

- **Вмісту розташування та умови пошуку**: переконайтеся, що ви вибрали правильне розташування вмісту та умови пошуку. Якщо ви запускали великих пошукових (з багатьох місцях), розглянути, розділивши його на кілька пошуки.

- **Частково індексуватися елементи**: [частково індексуватися елементи](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) з поштових скриньок включені в результатах пошуку оцінками. Однак, частково індексовані елементів із сайтів SharePoint і OneDrive не включаються пошук оцінку.

- **Пошуку невдачі**: під час пошуку великої кількості поштових скриньок (понад 100000 поштових скриньок), ви можете отримати пошук помилок, з кодів помилок, таких як CS008-009 і CS012-002). У цьому випадку, спробуйте повторити пошук лише невдалі вмісту місцях. Дивіться [цю статтю](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) за додатковою інформацією.
