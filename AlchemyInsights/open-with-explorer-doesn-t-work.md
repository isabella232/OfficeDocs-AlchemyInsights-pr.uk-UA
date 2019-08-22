---
title: Відкрити за допомогою провідника не працює
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 7680766b53bd5e85789375d3f9e9ab635780ec6c
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538510"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="b3618-102">Відкрити за допомогою провідника не працює</span><span class="sxs-lookup"><span data-stu-id="b3618-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="b3618-103">Якщо **Відкрити у провіднику** або **Перегляд у Файловому провіднику** не працює переконайтеся, WebClient служби **запущений** , виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="b3618-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="b3618-104">Наприклад, може тривати багато часу, щоб відкрити бібліотеки SharePoint або OneDrive, коли службу не запущено.</span><span class="sxs-lookup"><span data-stu-id="b3618-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="b3618-105">У полі пошуку Windows, тип запустити, виберіть запустити застосунок робочого стола, введіть Services. msc і виберіть **Enter**.</span><span class="sxs-lookup"><span data-stu-id="b3618-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="b3618-106">Прокрутіть вниз до служби WebClient і перегляньте стовпець **стан** .</span><span class="sxs-lookup"><span data-stu-id="b3618-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="b3618-107">Якщо стан служби WebClient ще не **запущено**, двічі клацніть служби, натисніть кнопку **Пуск**і натисніть кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="b3618-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="b3618-108">Підключити послугу, якщо це необхідно, вибираючи або **вручну** або **автоматично** в полі **Тип запуску** .</span><span class="sxs-lookup"><span data-stu-id="b3618-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="b3618-109">Для виправлення неполадок відкриття у Файловому провіднику, переглянути [відкриті у провіднику](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="b3618-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="b3618-110">Дослідіть синхронізації як краща альтернатива: [SharePoint синхронізації файлів з новим клієнтом синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="b3618-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

