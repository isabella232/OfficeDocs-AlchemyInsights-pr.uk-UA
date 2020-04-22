---
title: Відкрити за допомогою провідника не працює
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713055"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="6eb94-102">Відкрити за допомогою провідника не працює</span><span class="sxs-lookup"><span data-stu-id="6eb94-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="6eb94-103">Якщо **Відкрити за допомогою провідника** або **подання у Файловому провіднику** , не працює, переконайтеся, що службу WebClient налаштовано на **роботу** , виконавши наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="6eb94-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="6eb94-104">Наприклад, це може зайняти багато часу, щоб відкрити бібліотеку SharePoint або OneDrive, коли служба не працює.</span><span class="sxs-lookup"><span data-stu-id="6eb94-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="6eb94-105">У полі пошуку Windows введіть виконати, виберіть пункт запустити робочий стіл, введіть Services. msc, а потім виберіть **ввести**.</span><span class="sxs-lookup"><span data-stu-id="6eb94-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="6eb94-106">Прокрутіть униз до служби WebClient і перевірте стовпець **стан** .</span><span class="sxs-lookup"><span data-stu-id="6eb94-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="6eb94-107">Якщо стан служби WebClient не **запущено**, двічі клацніть службу, натисніть кнопку **Пуск**і натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="6eb94-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="6eb94-108">Увімкніть службу, якщо потрібно, вибравши пункт **вручну** або **автоматично** в полі **Тип запуску** .</span><span class="sxs-lookup"><span data-stu-id="6eb94-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="6eb94-109">Щоб усунути неполадки, які відкриваються у Файловому провіднику [, див.](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="6eb94-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="6eb94-110">Дослідіть синхронізацію як кращу альтернативу: [Синхронізація файлів SharePoint з новим клієнтом синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="6eb94-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

