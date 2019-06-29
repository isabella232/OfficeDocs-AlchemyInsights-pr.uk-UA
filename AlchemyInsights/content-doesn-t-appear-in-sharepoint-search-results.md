---
title: Вміст не відображається в результатах пошуку SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363847"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Вміст не відображається в результатах пошуку SharePoint

Виконайте такі дії під час очікуваних вміст не відображається в результатах пошуку.
  
1. Перевірте, що **сайт** , який містить очікуваного вмісту налаштовані не блокувати вміст з'являтися в результатах пошуку. Дотримуйтесь інструкцій у [відображення вмісту сайту в результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Перевірте, що **список** або **бібліотеку** , яка містить очікуваного вмісту налаштовані не блокувати вміст з'являтися в результатах пошуку. Дотримуйтесь інструкцій у [відображення вмісту списків або бібліотек в результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Переконайтеся, що сторінки, документ або Розмітка сторінки користувацькі публікуються на **основну версію.** Виконайте крок 3 в [пошуку не повертає всі результати в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Переконайтеся, що користувач має **права** дозволено переглянути зовнішній вміст. Виконайте дії у [розумінні рівнів дозволів в SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
    
5. Якщо пошук схему було змінено, додавши нову керовану властивість, відредагувавши керована властивість або шляхом видалення з керованою властивістю, тоді запит на сканування і повторно проіндексувати вимагатиметься. **Повторне індексування** вмісту, виконавши дії, зазначені в [Надіслати запит уручну сканування і повторно індексацію сайту, бібліотеку або список](https://docs.microsoft.com/sharepoint/crawl-site-content). Це може зайняти деякий час, зачекайте 24 години перед перевіркою результати знову.

Докладніше перегляньте [Увімкнути вміст на сайті, щоб бути придатним для пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
