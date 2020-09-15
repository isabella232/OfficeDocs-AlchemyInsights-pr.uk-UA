---
title: Виправлення неполадок із використанням функції "Відкрити у провіднику"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659079"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="c6c53-102">Виправлення неполадок із відкритою програмою "провідник"</span><span class="sxs-lookup"><span data-stu-id="c6c53-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="c6c53-103">Виправлення поширених проблем із відкриттям бібліотеки документів у SharePoint або OneDrive за допомогою команди " **Відкрити у провіднику** ":</span><span class="sxs-lookup"><span data-stu-id="c6c53-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="c6c53-104">Використовуйте браузер Internet Explorer 10 або Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="c6c53-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="c6c53-105">**Відкрити у провіднику** не сумісно з Microsoft EDGE, Google Chrome, Firefox та іншими користувачами.</span><span class="sxs-lookup"><span data-stu-id="c6c53-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c6c53-106">**Відкрити у провіднику** у всіх браузерах, окрім Internet Explorer, вимкнуто.</span><span class="sxs-lookup"><span data-stu-id="c6c53-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="c6c53-107">**Відкрити у провіднику** не можна в сучасному досвіді бібліотек SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c6c53-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="c6c53-108">Натомість використовуйте **подання у Файловому провіднику** .</span><span class="sxs-lookup"><span data-stu-id="c6c53-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="c6c53-109">Виберіть подання " **варіанти подання** " \> **у Файловому провіднику**.</span><span class="sxs-lookup"><span data-stu-id="c6c53-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="c6c53-110">Перегляд у Файловому провіднику не сумісний із Microsoft EDGE, Google Chrome, Firefox та іншими користувачами.</span><span class="sxs-lookup"><span data-stu-id="c6c53-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="c6c53-111">**Перегляд у Файловому провіднику** доступний лише в Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="c6c53-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="c6c53-112">Переконайтеся, що служба веб-клієнта працює.</span><span class="sxs-lookup"><span data-stu-id="c6c53-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="c6c53-113">У полі Пошук у Windows введіть Run (запустити), виберіть програму Run Desktop, введіть Services. msc, а потім натисніть клавішу ВВІД.</span><span class="sxs-lookup"><span data-stu-id="c6c53-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="c6c53-114">Прокрутіть униз до служби веб-клієнта та переконайтеся, що у стовпці **стан** відображається слово "запущено".</span><span class="sxs-lookup"><span data-stu-id="c6c53-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="c6c53-115">Якщо це не так, двічі клацніть службу, натисніть кнопку **Пуск**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="c6c53-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c6c53-116">(Можливо, спочатку потрібно ввімкнути службу, вибравши **вручну** або **автоматично** в полі **Тип запуску** .)</span><span class="sxs-lookup"><span data-stu-id="c6c53-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c6c53-117">Відкриття бібліотеки в Файловому провіднику зручно, якщо потрібно скопіювати або перемістити кілька файлів і папок, але якщо потрібно регулярно працювати в бібліотеці, радимо його синхронізувати.</span><span class="sxs-lookup"><span data-stu-id="c6c53-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="c6c53-118">Щоб виправити неполадки під час відкриття файлового провідника, [Відкрийте вікно відкрити у провіднику](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="c6c53-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c6c53-119">Докладні відомості про настроювання синхронізації наведено в статті [Синхронізація файлів SharePoint за допомогою нового клієнта синхронізації OneDrive](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="c6c53-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="c6c53-120">Перегляньте статтю [використання команди "Відкрити у провіднику", щоб виправити неполадки в службі SharePoint Online, щоб](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="c6c53-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

