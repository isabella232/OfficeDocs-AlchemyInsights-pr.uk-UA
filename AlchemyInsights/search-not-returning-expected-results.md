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
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="58d87-102">Пошук вмісту, не повертаються очікуваних результатів</span><span class="sxs-lookup"><span data-stu-id="58d87-102">Content Search not returning expected results</span></span>

<span data-ttu-id="58d87-103">Під час запуску пошуку вмісту з Microsoft 365 безпеки & центру підтримки, може з'явитися неочікувані результати пошуку.</span><span class="sxs-lookup"><span data-stu-id="58d87-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="58d87-104">Розглянемо наступні речі, які можуть вплинути на результати пошуку:</span><span class="sxs-lookup"><span data-stu-id="58d87-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="58d87-105">**Розташування вмісту та умови пошуку**: переконайтеся, що вибрано правильне розташування вмісту та умови пошуку.</span><span class="sxs-lookup"><span data-stu-id="58d87-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="58d87-106">Якщо ви запустили великий Пошук (з багатьма розташуваннями), розглянемо розділення його на кілька пошуків.</span><span class="sxs-lookup"><span data-stu-id="58d87-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="58d87-107">**Частково індексовані елементи**: [частково індексовані елементи](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) з поштових скриньок включаються до прогнозованого результату пошуку.</span><span class="sxs-lookup"><span data-stu-id="58d87-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="58d87-108">Проте частково індексовані елементи з сайтів у SharePoint і OneDrive не включаються в оцінку пошуку.</span><span class="sxs-lookup"><span data-stu-id="58d87-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="58d87-109">**Помилки пошуку**: під час пошуку великої кількості поштових скриньок (понад 100 000 поштових скриньок), ви можете отримати помилки пошуку, з кодами помилок, ТАКИМИ як CS008-009 і CS012-002).</span><span class="sxs-lookup"><span data-stu-id="58d87-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="58d87-110">У такому разі повторіть пошук лише для місць, де не вдалося знайти вміст.</span><span class="sxs-lookup"><span data-stu-id="58d87-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="58d87-111">Докладнішу інформацію наведено в [цій статті](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="58d87-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
