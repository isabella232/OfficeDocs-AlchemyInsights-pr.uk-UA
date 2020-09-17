---
title: Запитання про те, як використовувати засіб розгортання Office (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774912"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Запитання про те, як використовувати засіб розгортання Office (ODT)

Завантажте засіб розгортання Office з [центру завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Після завантаження файлу запустіть виконуваний файл самовидобування, який містить виконуваний засіб розгортання Office (setup.exe), а також зразок файлу конфігурації (configuration.xml).
  
 **Щоб виключити або видалити програми Microsoft 365 для корпоративних продуктів із клієнтських комп'ютерів, виконайте такі дії:**
  
Під час інсталяції програм Microsoft 365 для підприємств можна виключити певні продукти. Щоб виконати ці дії, виконайте вказівки з інсталяції пакета Office у форматі ODT, але додайте елемент ExcludeApp у файлі конфігурації. Наприклад, цей файл конфігурації інсталює всі програми Microsoft 365 для підприємств, окрім видавця:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Огляд засобу розгортання Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

