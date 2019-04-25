---
title: Питання про використання в офісі розгортання інструмент (у форматі ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e91d40f872dd401ee210ac05eb39d64b6fb88027
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371789"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="c7cc3-102">Питання про використання в офісі розгортання інструмент (у форматі ODT)</span><span class="sxs-lookup"><span data-stu-id="c7cc3-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="c7cc3-103">Завантажити засіб розгортання офісу з [Центру завантажень Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="c7cc3-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="c7cc3-104">Після завантаження файлу, запустити саморозпаковується виконуваний файл, який містить Office розгортання засобу виконувану (setup.exe) і зразок файлу конфігурації (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="c7cc3-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="c7cc3-105">**Виключити або видалення продуктів Office 365 ProPlus із клієнтськими комп'ютерами:**</span><span class="sxs-lookup"><span data-stu-id="c7cc3-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="c7cc3-106">Під час інсталяції Office 365 ProPlus, ви можете виключити певні продукти.</span><span class="sxs-lookup"><span data-stu-id="c7cc3-106">When installing Office 365 ProPlus, you can exclude specific products.</span></span> <span data-ttu-id="c7cc3-107">Для цього дотримуйтесь інструкцій з інсталяції Office з на: ODT, але включають ExcludeApp елементу у файлі конфігурації.</span><span class="sxs-lookup"><span data-stu-id="c7cc3-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="c7cc3-108">Наприклад, цей файл конфігурації встановлює Office 365 ProPlus продуктів Крім видавця:</span><span class="sxs-lookup"><span data-stu-id="c7cc3-108">For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="c7cc3-109">Огляд розгортання засобу Office</span><span class="sxs-lookup"><span data-stu-id="c7cc3-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  

