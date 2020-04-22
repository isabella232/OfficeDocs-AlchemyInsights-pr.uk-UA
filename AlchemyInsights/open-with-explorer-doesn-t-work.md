---
title: Відкрити за допомогою провідника не працює
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713055"
---
# <a name="open-with-explorer-isnt-working"></a>Відкрити за допомогою провідника не працює

Якщо **Відкрити за допомогою провідника** або **подання у Файловому провіднику** , не працює, переконайтеся, що службу WebClient налаштовано на **роботу** , виконавши наведені нижче дії. Наприклад, це може зайняти багато часу, щоб відкрити бібліотеку SharePoint або OneDrive, коли служба не працює. 
  
1. У полі пошуку Windows введіть виконати, виберіть пункт запустити робочий стіл, введіть Services. msc, а потім виберіть **ввести**.
    
2. Прокрутіть униз до служби WebClient і перевірте стовпець **стан** . Якщо стан служби WebClient не **запущено**, двічі клацніть службу, натисніть кнопку **Пуск**і натисніть кнопку **OK**. Увімкніть службу, якщо потрібно, вибравши пункт **вручну** або **автоматично** в полі **Тип запуску** . 
    
> [!NOTE]
> Щоб усунути неполадки, які відкриваються у Файловому провіднику [, див.](https://go.microsoft.com/fwlink/?linkid=871665) Дослідіть синхронізацію як кращу альтернативу: [Синхронізація файлів SharePoint з новим клієнтом синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666). 
  

