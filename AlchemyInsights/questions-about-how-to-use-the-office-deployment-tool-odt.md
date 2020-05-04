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
ms.openlocfilehash: 4aef42df4dde17d15863fca67e41f0ff23e506dc
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010779"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="d7aa0-102">Питання про те, як використовувати засіб розгортання Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="d7aa0-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="d7aa0-103">Завантажити засіб розгортання Office, з [центру завантажень Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="d7aa0-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="d7aa0-104">Після завантаження файлу, запустіть саморозпаковується виконуваний файл, який містить засіб розгортання Office, виконувані (Setup. exe) і зразок файлу конфігурації (Configuration. XML).</span><span class="sxs-lookup"><span data-stu-id="d7aa0-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="d7aa0-105">**Щоб виключити або видалити програми Microsoft 365 для корпоративних продуктів із клієнтських комп'ютерів:**</span><span class="sxs-lookup"><span data-stu-id="d7aa0-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="d7aa0-106">Під час інсталяції програм Microsoft 365 для підприємств можна виключити певні продукти.</span><span class="sxs-lookup"><span data-stu-id="d7aa0-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="d7aa0-107">Для цього виконайте вказівки з інсталяції Office за допомогою ODT, але додайте елемент ExcludeApp у файлі конфігурації.</span><span class="sxs-lookup"><span data-stu-id="d7aa0-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="d7aa0-108">Наприклад, цей файл конфігурації інсталює всі програми Microsoft 365 для корпоративних продуктів, крім Publisher:</span><span class="sxs-lookup"><span data-stu-id="d7aa0-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="d7aa0-109">Огляд засобу розгортання Office</span><span class="sxs-lookup"><span data-stu-id="d7aa0-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

