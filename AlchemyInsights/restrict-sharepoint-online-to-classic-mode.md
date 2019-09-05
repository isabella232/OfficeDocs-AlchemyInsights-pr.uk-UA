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
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752089"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Обмеження SharePoint Online на класичний режим

Деякі організації, як і раніше, вимагають класичний режим роботи. Хоча немає планів для видалення класичного режиму на рівні зернистих, більше не можна обмежити всю організацію (клієнта) в класичному режимі для списків і бібліотек.

Адміністратор матиме такі параметри для керування окремими списками та бібліотеками в класичному режимі за допомогою зернистих перемикачів, які ми надаємо на наступних рівнях:

- колекції сайтів
- Сайт
- Список
- Бібліотека

Крім того, списки, які використовують певні функції та настроювання, які не підтримуються сучасними, все одно буде автоматично переключається в класичний режим.

Починаючи з 1 квітня 2019, процес вимкнення рівня клієнта відмовитися від сучасних список і бібліотек почнеться і триватиме до 31 травня 2019.  Списки та бібліотеки, які перебувають у класичному режимі внаслідок відмови клієнта, автоматично зсуваються на сучасну.

Якщо вам потрібен класичний режим, будь ласка, дивіться більш детальну інформацію [тут](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) і ПНП PowerShell інструкція [тут](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , яка описує параметри та інструменти, які ви можете використовувати сьогодні, щоб використовувати класичний досвід режимі.
