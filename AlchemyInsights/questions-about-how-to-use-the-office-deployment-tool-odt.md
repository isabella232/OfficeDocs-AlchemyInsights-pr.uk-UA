---
title: Питання про використання в офісі розгортання інструмент (у форматі ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29496011"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Питання про використання в офісі розгортання інструмент (у форматі ODT)

Завантажити засіб розгортання офісу з [Центру завантажень Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Після завантаження файлу, запустити саморозпаковується виконуваний файл, який містить Office розгортання засобу виконувану (setup.exe) і зразок файлу конфігурації (configuration.xml).
  
 **Виключити або видалення продуктів Office 365 ProPlus із клієнтськими комп'ютерами:**
  
Під час інсталяції Office 365 ProPlus, ви можете виключити певні продукти. Для цього дотримуйтесь інструкцій з інсталяції Office з на: ODT, але включають ExcludeApp елементу у файлі конфігурації. Наприклад, цей файл конфігурації встановлює Office 365 ProPlus продуктів Крім видавця:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Огляд розгортання засобу Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

