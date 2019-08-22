---
title: Відкрити за допомогою провідника не працює
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538510"
---
# <a name="open-with-explorer-isnt-working"></a>Відкрити за допомогою провідника не працює

Якщо **Відкрити у провіднику** або **Перегляд у Файловому провіднику** не працює переконайтеся, WebClient служби **запущений** , виконавши наведені нижче дії. Наприклад, може тривати багато часу, щоб відкрити бібліотеки SharePoint або OneDrive, коли службу не запущено. 
  
1. У полі пошуку Windows, тип запустити, виберіть запустити застосунок робочого стола, введіть Services. msc і виберіть **Enter**.
    
2. Прокрутіть вниз до служби WebClient і перегляньте стовпець **стан** . Якщо стан служби WebClient ще не **запущено**, двічі клацніть служби, натисніть кнопку **Пуск**і натисніть кнопку **ОК**. Підключити послугу, якщо це необхідно, вибираючи або **вручну** або **автоматично** в полі **Тип запуску** . 
    
> [!NOTE]
> Для виправлення неполадок відкриття у Файловому провіднику, переглянути [відкриті у провіднику](https://go.microsoft.com/fwlink/?linkid=871665). Дослідіть синхронізації як краща альтернатива: [SharePoint синхронізації файлів з новим клієнтом синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

