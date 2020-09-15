---
title: Вміст не відображається в результатах пошуку в службі SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713151"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Вміст не відображається в результатах пошуку в службі SharePoint

Виконайте ці кроки з виправлення неполадок, коли очікуваний вміст не відображається в результатах пошуку.
  
1. Переконайтеся, що для **сайту** , який містить очікуваний вміст, установіть прапорець Дозволити вміст відображатися в результатах пошуку. Виконайте вказівки, описані в розділі [відображення вмісту на сайті в результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Переконайтеся, що для **списку** або **бібліотеки** , яка містить очікуваний вміст, установіть прапорець Дозволити вміст відображатися в результатах пошуку. Виконайте вказівки, описані в розділі [відображення вмісту зі списків або бібліотек у результатах пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Переконайтеся, що для сторінки, документа або настроюваного макета сторінки Опубліковано як **Основна версія.** Виконайте крок 3 в [результатах пошуку, не повертають всі результати в службі SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).

4. Переконайтеся, що користувач має **дозволи** на перегляд вмісту. Виконайте вказівки, описані в статті [Загальні відомості про рівні дозволів у службі SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
    
5. Якщо схему пошуку змінено, додавши нову керовану властивість, редагуючи керовану властивість, або видаливши керовану властивість, а потім потрібно буде виконати запит на обхід та повторно індексувати. **Повторно індексувати** вміст, виконавши вказівки, описані в [запиті вручну обхід та повторне індексування сайту, бібліотеки або списку](https://docs.microsoft.com/sharepoint/crawl-site-content). Це може тривати деякий час, зачекайте 24 години, перш ніж знову перевірити результати.

Докладні відомості наведено в статті [Увімкнення вмісту сайту для пошуку](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
