---
title: Виправлення неполадок, пов'язаних із використанням програми "Відкрити за допомогою провідника"
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
ms.openlocfilehash: a9ab7dd27e4dc1bd76c93cc81260616063e638ed
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742754"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="e92bd-102">Вирішення проблем із відкритими за допомогою провідника</span><span class="sxs-lookup"><span data-stu-id="e92bd-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="e92bd-103">Вирішення поширених проблем із відкриттям бібліотеки документів у SharePoint або OneDrive за допомогою команди **Відкрити за допомогою провідника** :</span><span class="sxs-lookup"><span data-stu-id="e92bd-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="e92bd-104">Використовуйте Internet Explorer 10 або Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="e92bd-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="e92bd-105">**Відкрити за допомогою провідника** не сумісний з Microsoft EDGE, Google Chrome, Firefox та інші.</span><span class="sxs-lookup"><span data-stu-id="e92bd-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e92bd-106">**Відкрити за допомогою провідника** вимкнуто у всіх браузерах, крім Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="e92bd-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="e92bd-107">**Відкрити за допомогою провідника** недоступний у сучасному досвіді для бібліотек SharePoint.</span><span class="sxs-lookup"><span data-stu-id="e92bd-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="e92bd-108">Натомість використовуйте **подання у Файловому провіднику** .</span><span class="sxs-lookup"><span data-stu-id="e92bd-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="e92bd-109">Виберіть Перегляд **параметрів** \> перегляд **у Файловому провіднику**.</span><span class="sxs-lookup"><span data-stu-id="e92bd-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="e92bd-110">Перегляд у Файловому провіднику несумісний із Microsoft EDGE, Google Chrome, Firefox та іншими користувачами.</span><span class="sxs-lookup"><span data-stu-id="e92bd-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="e92bd-111">**Перегляд у Файловому провіднику** , доступний лише у браузері Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="e92bd-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="e92bd-112">Переконайтеся, що запущено службу WebClient.</span><span class="sxs-lookup"><span data-stu-id="e92bd-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="e92bd-113">У полі пошуку Windows введіть виконати, виберіть програму робочого стола, введіть Services. msc і натисніть клавішу ENTER.</span><span class="sxs-lookup"><span data-stu-id="e92bd-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="e92bd-114">Прокрутіть униз до служби WebClient і переконайтеся, що у стовпці **стан** відображається "запущено".</span><span class="sxs-lookup"><span data-stu-id="e92bd-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="e92bd-115">Якщо це не так, двічі клацніть службу, натисніть кнопку **Пуск**і натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="e92bd-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="e92bd-116">(Можливо, потрібно спочатку ввімкнути службу, вибравши в полі **Тип запуску** пункт **вручну** або **автоматично** .)</span><span class="sxs-lookup"><span data-stu-id="e92bd-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="e92bd-117">Відкриття бібліотеки у Файловому провіднику зручно, якщо потрібно скопіювати або перемістити кілька файлів і папок, але якщо потрібно регулярно працювати в бібліотеці, радимо її синхронізувати.</span><span class="sxs-lookup"><span data-stu-id="e92bd-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="e92bd-118">Щоб усунути неполадки, які відкриваються у Файловому провіднику [, див.](https://go.microsoft.com/fwlink/?linkid=871665)</span><span class="sxs-lookup"><span data-stu-id="e92bd-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="e92bd-119">Відомості про настроювання синхронізації наведено в полі [Синхронізація файлів SharePoint із новим клієнтом синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="e92bd-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="e92bd-120">Будь ласка, перегляньте статтю [як використовувати команду "Відкрити за допомогою провідника" для виправлення неполадок у SharePoint Online, щоб](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) отримати додаткові відомості.</span><span class="sxs-lookup"><span data-stu-id="e92bd-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

