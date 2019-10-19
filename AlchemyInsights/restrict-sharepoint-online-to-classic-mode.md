---
title: Обмеження SharePoint Online на класичний режим
ms.author: pebaum
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 18d263593d99f24c3020336ae601df14dbbf5411
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36752089"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="57570-102">Обмеження SharePoint Online на класичний режим</span><span class="sxs-lookup"><span data-stu-id="57570-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="57570-103">Деякі організації, як і раніше, вимагають класичний режим роботи.</span><span class="sxs-lookup"><span data-stu-id="57570-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="57570-104">Хоча немає планів для видалення класичного режиму на рівні зернистих, більше не можна обмежити всю організацію (клієнта) в класичному режимі для списків і бібліотек.</span><span class="sxs-lookup"><span data-stu-id="57570-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="57570-105">Адміністратор матиме такі параметри для керування окремими списками та бібліотеками в класичному режимі за допомогою зернистих перемикачів, які ми надаємо на наступних рівнях:</span><span class="sxs-lookup"><span data-stu-id="57570-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="57570-106">колекції сайтів</span><span class="sxs-lookup"><span data-stu-id="57570-106">site collection</span></span>
- <span data-ttu-id="57570-107">Сайт</span><span class="sxs-lookup"><span data-stu-id="57570-107">site</span></span>
- <span data-ttu-id="57570-108">Список</span><span class="sxs-lookup"><span data-stu-id="57570-108">list</span></span>
- <span data-ttu-id="57570-109">Бібліотека</span><span class="sxs-lookup"><span data-stu-id="57570-109">library</span></span>

<span data-ttu-id="57570-110">Крім того, списки, які використовують певні функції та настроювання, які не підтримуються сучасними, все одно буде автоматично переключається в класичний режим.</span><span class="sxs-lookup"><span data-stu-id="57570-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="57570-111">Починаючи з 1 квітня 2019, процес вимкнення рівня клієнта відмовитися від сучасних список і бібліотек почнеться і триватиме до 31 травня 2019.</span><span class="sxs-lookup"><span data-stu-id="57570-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="57570-112">Списки та бібліотеки, які перебувають у класичному режимі внаслідок відмови клієнта, автоматично зсуваються на сучасну.</span><span class="sxs-lookup"><span data-stu-id="57570-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="57570-113">Якщо вам потрібен класичний режим, будь ласка, дивіться більш детальну інформацію [тут](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) і ПНП PowerShell інструкція [тут](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , яка описує параметри та інструменти, які ви можете використовувати сьогодні, щоб використовувати класичний досвід режимі.</span><span class="sxs-lookup"><span data-stu-id="57570-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
