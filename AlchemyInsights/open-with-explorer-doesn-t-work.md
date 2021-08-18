---
title: Не вдається відкрити у провіднику
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
ms.openlocfilehash: 2ba6f08b40dd194bf1ffd9a455a134a2fc553b51
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321882"
---
# <a name="open-with-explorer-isnt-working"></a>"Відкрити у провіднику" не працює

Якщо параметр Відкрити  **у провіднику** або Переглянути у Файловому провіднику не працює, переконайтеся, що для служби WebClient установлено значення **Запуск,** виконавши наведені нижче дії. Наприклад, відкриття бібліотеки SharePoint або OneDrive, коли службу не запущено, може знадобити багато часу. 
  
1. У полі Windows введіть виконати, виберіть класичну програму Run, введіть services.msc, а потім натисніть **клавішу Enter**.
    
2. Прокрутіть сторінку вниз до служби WebClient і перевірте **стовпець Стан.** Якщо стан служби WebClient не запущено, двічі клацніть службу, натисніть кнопку **Пуск** і натисніть кнопку **OK.** За потреби ввімкніть  службу, вибравши в полі Тип запуску значення Вручну **або Автоматично.**  
    
**Примітка. Щоб дізнатися,** як вирішити проблеми з відкриттям у Файловому провіднику, див. [розділ "Відкрити у провіднику".](https://go.microsoft.com/fwlink/?linkid=871665) Дізнайтеся, як покращити синхронізацію. [Синхронізуйте SharePoint файлів за допомогою нового синхронізатор OneDrive клієнта.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

