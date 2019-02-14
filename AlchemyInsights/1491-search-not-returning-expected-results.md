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
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964995"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="782f8-102">Пошук за змістом не повертаючи очікувані результати</span><span class="sxs-lookup"><span data-stu-id="782f8-102">Content Search not returning expected results</span></span>

<span data-ttu-id="782f8-p101">Під час пошуків вмісту з Office 365 безпеки & центрі дотримання, може з'явитися несподіваних результатів. Розглянути наступні речі, які можуть вплинути на результати пошуку:</span><span class="sxs-lookup"><span data-stu-id="782f8-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="782f8-p102">**Вмісту розташування та умови пошуку**: переконайтеся, що ви вибрали правильне розташування вмісту та умови пошуку. Якщо ви запускали великих пошукових (з багатьох місцях), розглянути, розділивши його на кілька пошуки.</span><span class="sxs-lookup"><span data-stu-id="782f8-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="782f8-p103">**Частково індексуватися елементи**: [частково індексуватися елементи](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) з поштових скриньок включені в результатах пошуку оцінками. Однак, частково індексовані елементів із сайтів SharePoint і OneDrive не включаються пошук оцінку.</span><span class="sxs-lookup"><span data-stu-id="782f8-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="782f8-p104">**Пошуку невдачі**: під час пошуку великої кількості поштових скриньок (понад 100000 поштових скриньок), ви можете отримати пошук помилок, з кодів помилок, таких як CS008-009 і CS012-002). У цьому випадку, спробуйте повторити пошук лише невдалі вмісту місцях. Дивіться [цю статтю](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) за додатковою інформацією.</span><span class="sxs-lookup"><span data-stu-id="782f8-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
