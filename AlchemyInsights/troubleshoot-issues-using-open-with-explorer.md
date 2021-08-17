---
title: Усунення несправностей, пов'язаних із використанням функції "Відкрити у провідни
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 0cbcfb506295d5732f7109be7a103bbdef530a529c7408c6d9d45a7b38a89915
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54048177"
---
# <a name="fix-problems-with-open-with-explorer"></a>Вирішення проблем із відкриттям у провіднику

Вирішення поширених проблем із відкриттям бібліотеки документів у SharePoint або OneDrive за допомогою команди Відкрити у **провіднику:** 
  
- Використовуйте Internet Explorer 10 або Internet Explorer 11. **"Відкрити у** провіднику" несумісний із Microsoft Edge, Google Chrome, Firefox та іншими користувачами. **Параметр "Відкрити у провіднику"** вимкнуто в усіх браузерах, крім Internet Explorer. 
    
- **"Відкрити у** провіднику" недоступне у сучасному SharePoint бібліотек. **Натомість скористайтеся поданням у Файловому** провіднику. Виберіть **Параметри подання Переглянути** у \> **Файловому провіднику**. Перегляд у Файловому провіднику несумісний із Microsoft Edge, Google Chrome, Firefox та іншими програмами. **Перегляд у Файловому провіднику** доступний лише в Internet Explorer. 
    
- Переконайтеся, що службу WebClient запущено. У полі Windows введіть виконати, виберіть класичну програму Run, введіть services.msc, а потім натисніть клавішу Enter. Прокрутіть униз до служби WebClient і переконайтеся, що у стовпці **Стан** відображається "Запущено". Якщо це не так, двічі клацніть службу, натисніть кнопку **Пуск** і натисніть кнопку **OK.** (Можливо, спочатку знадобиться активувати  службу, вибравши в полі Тип запуску значення Вручну **або Автоматично.)**  
    
> [!NOTE]
> Відкрити бібліотеку у Файловому провіднику зручно, якщо потрібно копіювати або переміщати кілька файлів і папок один раз, але якщо вам потрібно регулярно працювати в бібліотеці, радимо синхронізувати її. Відомості про виправлення неполадок, пов'язаних із відкриттям у [Файловому провіднику, див. в цьому провіднику.](https://go.microsoft.com/fwlink/?linkid=871665) Відомості про налаштування синхронізації див. в [SharePoint синхронізації файлів за допомогою нового синхронізатор OneDrive клієнта.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Докладні відомості див. в статті Використання команди "Відкрити у провіднику" SharePoint [Online.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 
  

