---
title: Усунення несправностей відкрити за допомогою провідника
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759315"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="9f8b9-102">Вирішення проблем із відкритим з провідника</span><span class="sxs-lookup"><span data-stu-id="9f8b9-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="9f8b9-103">Вирішення поширених проблем із відкриття бібліотеки документів SharePoint або OneDrive за допомогою команди **Відкрити у провіднику** :</span><span class="sxs-lookup"><span data-stu-id="9f8b9-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="9f8b9-104">Використовувати Internet Explorer 10 або Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="9f8b9-105">**Відкрити у провіднику** несумісний з Microsoft краю, Google Chrome, Firefox та інших.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9f8b9-106">**Відкрити у провіднику** вимикається у всіх браузерах Крім Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="9f8b9-107">**Відкрити у провіднику** недоступна в сучасних досвід для бібліотеки SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="9f8b9-108">Слід використовувати **подання у Файловому провіднику** .</span><span class="sxs-lookup"><span data-stu-id="9f8b9-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="9f8b9-109">Виберіть **Параметри подання** \> **подання у Файловому провіднику**.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="9f8b9-110">Перегляд у Файловому провіднику несумісний з Microsoft краю, Google Chrome, Firefox та інших.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="9f8b9-111">**Перегляд у Файловому провіднику** в лише у браузері Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="9f8b9-112">Переконайтеся, що службу WebClient запущено.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="9f8b9-113">У полі пошуку Windows введіть виконати, виберіть запустити застосунок робочого стола, введіть Services. msc і натисніть клавішу Enter.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="9f8b9-114">Прокрутіть вниз до служби WebClient і переконайтеся, що у стовпці **стан** відображено "Running".</span><span class="sxs-lookup"><span data-stu-id="9f8b9-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="9f8b9-115">Якщо цього не відбувається, двічі клацніть служби, натисніть кнопку **запустити**і натисніть кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9f8b9-116">(Можливо, вам потрібно спочатку ввімкнути службу, вибравши або **вручну** або **автоматично** в полі **Тип запуску** .)</span><span class="sxs-lookup"><span data-stu-id="9f8b9-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9f8b9-117">Відкриття бібліотеки у Файловому провіднику це зручно, якщо потрібно скопіювати або перемістити кілька файлів і папок, один раз, але якщо ви хочете регулярно працювати в бібліотеці, ми рекомендуємо її синхронізацію.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="9f8b9-118">Для виправлення неполадок відкриття у Файловому провіднику, переглянути [відкриті у провіднику](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="9f8b9-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9f8b9-119">Інформація щодо настроювання синхронізації наведено [SharePoint синхронізації файлів з новим клієнтом синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="9f8b9-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="9f8b9-120">Будь ласка, перегляньте статтю [як за допомогою команди "з провідник" для виправлення неполадок у SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) за додатковою інформацією.</span><span class="sxs-lookup"><span data-stu-id="9f8b9-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

