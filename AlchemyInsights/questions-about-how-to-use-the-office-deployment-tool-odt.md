---
title: Запитання про використання засобу Office розгортання (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959704"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Запитання про використання засобу Office розгортання (ODT)

Завантажте засіб Office розгортання з [Центру завантажень Microsoft.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Після завантаження файлу запустіть виконуваний файл із самостійним видобуванням виконуваного файлу, який містить виконуваний Office Deployment Tool (setup.exe) і зразок файлу конфігурації (configuration.xml).
  
 **Щоб виключити або Програми Microsoft 365 для підприємств продуктів із клієнтських комп'ютерів:**
  
Під час Програми Microsoft 365 для підприємств продуктів можна виключити певні продукти. Для цього виконайте вказівки з інсталяції Office ODT, але в файл конфігурації додайте елемент ExcludeApp. Наприклад, цей файл конфігурації інсталює всі продукти Програми Microsoft 365 для підприємств, крім Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Огляд засобу Office розгортання](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

