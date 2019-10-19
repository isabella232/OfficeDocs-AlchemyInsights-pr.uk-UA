---
title: Питання про те, як використовувати засіб розгортання Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 604fc200517316de6e0194bd64e6eb3039cfa61b
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36553561"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Питання про те, як використовувати засіб розгортання Office (ODT)

Завантажити засіб розгортання Office, з [центру завантажень Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Після завантаження файлу, запустіть саморозпаковується виконуваний файл, який містить засіб розгортання Office, виконувані (Setup. exe) і зразок файлу конфігурації (Configuration. XML).
  
 **Щоб виключити або видалити продукти Office 365 ProPlus з клієнтських комп'ютерів:**
  
Під час інсталяції Office 365 ProPlus можна виключити певні продукти. Для цього виконайте вказівки з інсталяції Office за допомогою ODT, але додайте елемент ExcludeApp у файлі конфігурації. Наприклад, цей конфігураційний файл інсталює всі продукти Office 365 ProPlus, крім видавців:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

