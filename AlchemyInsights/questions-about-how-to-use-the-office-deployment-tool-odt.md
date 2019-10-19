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
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="de8a9-102">Питання про те, як використовувати засіб розгортання Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="de8a9-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="de8a9-103">Завантажити засіб розгортання Office, з [центру завантажень Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="de8a9-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="de8a9-104">Після завантаження файлу, запустіть саморозпаковується виконуваний файл, який містить засіб розгортання Office, виконувані (Setup. exe) і зразок файлу конфігурації (Configuration. XML).</span><span class="sxs-lookup"><span data-stu-id="de8a9-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="de8a9-105">**Щоб виключити або видалити продукти Office 365 ProPlus з клієнтських комп'ютерів:**</span><span class="sxs-lookup"><span data-stu-id="de8a9-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="de8a9-106">Під час інсталяції Office 365 ProPlus можна виключити певні продукти.</span><span class="sxs-lookup"><span data-stu-id="de8a9-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="de8a9-107">Для цього виконайте вказівки з інсталяції Office за допомогою ODT, але додайте елемент ExcludeApp у файлі конфігурації.</span><span class="sxs-lookup"><span data-stu-id="de8a9-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="de8a9-108">Наприклад, цей конфігураційний файл інсталює всі продукти Office 365 ProPlus, крім видавців:</span><span class="sxs-lookup"><span data-stu-id="de8a9-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="de8a9-109">Огляд засобу розгортання Office</span><span class="sxs-lookup"><span data-stu-id="de8a9-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

