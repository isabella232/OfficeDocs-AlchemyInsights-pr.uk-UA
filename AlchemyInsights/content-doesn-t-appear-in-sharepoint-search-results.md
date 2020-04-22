---
title: Вміст не відображається в результатах пошуку SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a21e0047b41390f740f9e13d31cba32b13990151
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705682"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Вміст не відображається в результатах пошуку SharePoint

Виконайте ці кроки з виправлення неполадок, коли очікуваний вміст не відображається в результатах пошуку:
  
1. Переконайтеся, що на **сайті** , який містить очікуваний вміст налаштовано на дозволити вміст з'являтися в результатах пошуку. Дотримуйтеся вказівок у [показі вмісту на сайті в результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Переконайтеся, що **список** або **бібліотеку** , що містить очікуваний вміст, налаштовано на дозвіл на відображення вмісту в результатах пошуку. Дотримуйтеся вказівок у [списку Показати вміст із списків або бібліотек у результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Переконайтеся, що сторінка, документ або Настроювана Розмітка сторінки публікується як **Основна версія.** Дотримуйтесь крок 3 в [пошуку не повертає всі результати в SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Переконайтеся, що користувач має **дозволи** на перегляд вмісту. Виконайте дії, описані в [розумінні рівнів дозволів у SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Якщо схему пошуку змінено, додавши нову керовану властивість, відредагувавши керовану властивість або видаливши керовану властивість, потрібно буде виконати запит на обхід і повторне індексування. **Повторно індексувати** вміст, виконавши дії, зазначені в [ручному запиті на сканування та повторну індексацію сайту, бібліотеки або списку](https://docs.microsoft.com/sharepoint/crawl-site-content). Це може зайняти деякий час, зачекайте 24 години, перш ніж знову перевірити результати.

Докладніші відомості наведено в розділі [Увімкнення вмісту на сайті для пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
