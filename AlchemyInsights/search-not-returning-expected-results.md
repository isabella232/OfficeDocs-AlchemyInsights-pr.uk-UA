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
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="91ab0-102">Пошук вмісту не повертає очікувані результати</span><span class="sxs-lookup"><span data-stu-id="91ab0-102">Content Search not returning expected results</span></span>

<span data-ttu-id="91ab0-103">Під час виконання пошуків вмісту з центру відповідності & безпеки Microsoft 365 може з'явитися несподівані результати пошуку.</span><span class="sxs-lookup"><span data-stu-id="91ab0-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="91ab0-104">Зверніть увагу на наведені нижче дії, які можуть вплинути на результати пошуку.</span><span class="sxs-lookup"><span data-stu-id="91ab0-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="91ab0-105">**Розташування вмісту та умови пошуку**: переконайтеся, що вибрано відповідні розташування вмісту та умови пошуку.</span><span class="sxs-lookup"><span data-stu-id="91ab0-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="91ab0-106">Якщо ви запускали великий Пошук (з багатьма розташуваннями), спробуйте розділити її на кілька пошуків.</span><span class="sxs-lookup"><span data-stu-id="91ab0-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="91ab0-107">**Частково індексовані об'єкти**:  [частково індексовані об'єкти](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) з поштових скриньок включаються до оціночних результатів пошуку.</span><span class="sxs-lookup"><span data-stu-id="91ab0-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="91ab0-108">Проте частково індексовані об'єкти з сайтів у службі SharePoint і OneDrive не включаються в оціночну оцінку.</span><span class="sxs-lookup"><span data-stu-id="91ab0-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="91ab0-109">Помилки **пошуку**: під час пошуку великої кількості поштових скриньок (понад 100 000 поштових скриньок) ви можете отримати повідомлення про помилку пошуку з кодами помилок, наприклад CS008-009 і CS012-002).</span><span class="sxs-lookup"><span data-stu-id="91ab0-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="91ab0-110">У цьому випадку повторіть пошук лише для невиконаних розташувань вмісту.</span><span class="sxs-lookup"><span data-stu-id="91ab0-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="91ab0-111">Перегляньте  [цю статтю](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) , щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="91ab0-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
