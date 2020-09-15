---
title: Відкрити у провіднику не працює
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694477"
---
# <a name="open-with-explorer-isnt-working"></a>Відкрити у провіднику не працює

Якщо **Відкрити за допомогою провідника** або **подання у Файловому провіднику** , переконайтеся, що службу веб-клієнта настроєно на **Запуск** , виконавши наведені нижче дії. Наприклад, це може тривати довгий час, щоб відкрити бібліотеку SharePoint або OneDrive, коли служба не працює. 
  
1. У полі Пошук у Windows введіть Run (запустити), виберіть програму Run Desktop, введіть Services. msc, а потім натисніть кнопку **ввести**.
    
2. Прокрутіть униз до служби веб-клієнта та перевірте стовпець **стан** . Якщо стан служби веб-клієнта не **запущено**, двічі клацніть службу, натисніть кнопку **Пуск**, а потім натисніть кнопку **OK**. Активуйте службу, якщо потрібно, виберіть **вручну** або **автоматично** в полі **Тип запуску** . 
    
> [!NOTE]
> Щоб виправити неполадки під час відкриття файлового провідника, [Відкрийте вікно відкрити у провіднику](https://go.microsoft.com/fwlink/?linkid=871665). Дізнайтеся, як зручніше синхронізувати: [Синхронізація файлів SharePoint за допомогою нового клієнта синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

