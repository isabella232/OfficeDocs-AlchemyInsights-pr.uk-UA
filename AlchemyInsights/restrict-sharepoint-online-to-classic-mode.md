---
title: Обмеження служби SharePoint Online на класичний режим
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751444"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>Обмеження служби SharePoint Online на класичний режим

Деякі організації все ще вимагають класичного режиму роботи. Хоча немає планів, щоб видалити класичний режим на гранульованому рівні, не можна обмежувати всю організацію (клієнта) у класичному режимі для списків і бібліотек.

Адміністратор матиме наведені нижче параметри, щоб керувати окремими списками та бібліотеками в класичному режимі, використовуючи перемикачі гранульовані вимкнення, які ми надаємо на таких рівнях:

- Колекція сайтів
- сайт
- списку
- бібліотеки

Крім того, списки, які використовують певні функції та настройки, які не підтримуються в сучасному режимі, все одно буде автоматично змінено на класичний режим.

Починаючи з 1 квітня 2019, процес вимкнення рівня клієнта вимкнення сучасного списку та бібліотек розпочнеться і продовжиться до 31 травня 2019.  Списки та бібліотеки, які знаходяться в класичному режимі в результаті вимкнення клієнта, автоматично зсуваються до сучасних.

Якщо вам потрібен класичний режим, ознайомтеся з додатковими відомостями [тут](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) та інструкцією з PowerShell PnP, що описує варіанти та засоби [, які можна](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) використовувати сьогодні, щоб використовувати класичний режим роботи.
