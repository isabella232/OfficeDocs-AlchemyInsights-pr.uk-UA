---
title: Запитання про використання засобу розгортання Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790353"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Запитання про використання засобу розгортання Office (ODT)

Завантажте засіб розгортання Office із [Центру завантажень Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Після завантаження файлу запустіть виконуваний файл із виконуваним файлом із виконуваним засобом розгортання Office (setup.exe) і файлом зразка конфігурації (configuration.xml).
  
 **Щоб вилучити або вилучити програми Microsoft 365 для корпоративних продуктів із клієнтських комп'ютерів:**
  
Під час інсталяції програм Microsoft 365 для підприємств можна виключити певні продукти. Для цього дотримуйтеся вказівок з інсталяції Office із ODT, але додайте елемент ExcludeApp до файлу конфігурації. Наприклад, цей файл конфігурації інсталює всі програми Microsoft 365 для корпоративних продуктів, крім Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

