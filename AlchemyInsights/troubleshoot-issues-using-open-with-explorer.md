---
title: Усунення несправностей відкрити за допомогою провідника
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661772"
---
# <a name="fix-problems-with-open-with-explorer"></a>Вирішення проблем із відкритим з провідника

Вирішення поширених проблем із відкриття бібліотеки документів SharePoint або OneDrive за допомогою команди **Відкрити у провіднику** : 
  
- Використовувати Internet Explorer 10 або Internet Explorer 11. **Відкрити у провіднику** несумісний з Microsoft краю, Google Chrome, Firefox та інших. **Відкрити у провіднику** вимикається у всіх браузерах Крім Internet Explorer. 
    
- **Відкрити у провіднику** недоступна в сучасних досвід для бібліотеки SharePoint. Слід використовувати **подання у Файловому провіднику** . Виберіть **Параметри подання** \> **подання у Файловому провіднику**. Перегляд у Файловому провіднику несумісний з Microsoft краю, Google Chrome, Firefox та інших. **Перегляд у Файловому провіднику** в лише у браузері Internet Explorer. 
    
- Переконайтеся, що службу WebClient запущено. У полі пошуку Windows введіть виконати, виберіть запустити застосунок робочого стола, введіть Services. msc і натисніть клавішу Enter. Прокрутіть вниз до служби WebClient і переконайтеся, що у стовпці **стан** відображено "Running". Якщо цього не відбувається, двічі клацніть служби, натисніть кнопку **запустити**і натисніть кнопку **ОК**. (Можливо, вам потрібно спочатку ввімкнути службу, вибравши або **вручну** або **автоматично** в полі **Тип запуску** .) 
    
> [!NOTE]
> Відкриття бібліотеки у Файловому провіднику це зручно, якщо потрібно скопіювати або перемістити кілька файлів і папок, один раз, але якщо ви хочете регулярно працювати в бібліотеці, ми рекомендуємо її синхронізацію. Для виправлення неполадок відкриття у Файловому провіднику, переглянути [відкриті у провіднику](https://go.microsoft.com/fwlink/?linkid=871665). Інформація щодо настроювання синхронізації наведено [SharePoint синхронізації файлів з новим клієнтом синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).
  
Будь ласка, перегляньте статтю [як за допомогою команди "з провідник" для виправлення неполадок у SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) за додатковою інформацією. 
  

