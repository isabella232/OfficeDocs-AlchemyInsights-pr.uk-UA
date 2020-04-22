---
title: Питання про те, як використовувати засіб розгортання Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 96d3f70f554f71c43d6458ec8debc099cd9fb040
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43698079"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Питання про те, як використовувати засіб розгортання Office (ODT)

Завантажити засіб розгортання Office, з [центру завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Після завантаження файлу, запустіть саморозпаковується виконуваний файл, який містить засіб розгортання Office, виконувані (Setup. exe) і зразок файлу конфігурації (Configuration. XML).
  
 **Щоб виключити або видалити програми Microsoft 365 для корпоративних продуктів із клієнтських комп'ютерів:**
  
Під час інсталяції програм Microsoft 365 для підприємств можна виключити певні продукти. Для цього виконайте вказівки з інсталяції Office за допомогою ODT, але додайте елемент ExcludeApp у файлі конфігурації. Наприклад, цей файл конфігурації інсталює всі програми Microsoft 365 для корпоративних продуктів, крім Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

