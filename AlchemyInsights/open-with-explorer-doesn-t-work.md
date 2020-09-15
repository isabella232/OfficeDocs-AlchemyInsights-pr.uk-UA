---
title: Відкрити у провіднику не працює
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694477"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="8863d-102">Відкрити у провіднику не працює</span><span class="sxs-lookup"><span data-stu-id="8863d-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="8863d-103">Якщо **Відкрити за допомогою провідника** або **подання у Файловому провіднику** , переконайтеся, що службу веб-клієнта настроєно на **Запуск** , виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="8863d-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="8863d-104">Наприклад, це може тривати довгий час, щоб відкрити бібліотеку SharePoint або OneDrive, коли служба не працює.</span><span class="sxs-lookup"><span data-stu-id="8863d-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="8863d-105">У полі Пошук у Windows введіть Run (запустити), виберіть програму Run Desktop, введіть Services. msc, а потім натисніть кнопку **ввести**.</span><span class="sxs-lookup"><span data-stu-id="8863d-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="8863d-106">Прокрутіть униз до служби веб-клієнта та перевірте стовпець **стан** .</span><span class="sxs-lookup"><span data-stu-id="8863d-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="8863d-107">Якщо стан служби веб-клієнта не **запущено**, двічі клацніть службу, натисніть кнопку **Пуск**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="8863d-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8863d-108">Активуйте службу, якщо потрібно, виберіть **вручну** або **автоматично** в полі **Тип запуску** .</span><span class="sxs-lookup"><span data-stu-id="8863d-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8863d-109">Щоб виправити неполадки під час відкриття файлового провідника, [Відкрийте вікно відкрити у провіднику](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="8863d-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8863d-110">Дізнайтеся, як зручніше синхронізувати: [Синхронізація файлів SharePoint за допомогою нового клієнта синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="8863d-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

