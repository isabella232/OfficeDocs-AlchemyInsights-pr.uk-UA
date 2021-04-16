---
title: Засіб експорту витребування електронної пошти
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814609"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="33a92-102">Не вдається інсталювати або запустити засіб експорту витребування електронної даних?</span><span class="sxs-lookup"><span data-stu-id="33a92-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="33a92-103">Якщо не вдається інсталювати або запустити засіб експорту витребування електронної даних, щоб завантажити результати пошуку, перевірте таке:</span><span class="sxs-lookup"><span data-stu-id="33a92-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="33a92-104">Використовується комп'ютер, відповідає таким вимогам:</span><span class="sxs-lookup"><span data-stu-id="33a92-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="33a92-105">32- або 64-розрядна версія Windows 7 і пізніших версій</span><span class="sxs-lookup"><span data-stu-id="33a92-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="33a92-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="33a92-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="33a92-107">Підтримуваний браузер:</span><span class="sxs-lookup"><span data-stu-id="33a92-107">A supported browser:</span></span>

  - <span data-ttu-id="33a92-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="33a92-108">Microsoft Edge</span></span>

    <span data-ttu-id="33a92-109">Або</span><span class="sxs-lookup"><span data-stu-id="33a92-109">Or</span></span>

  - <span data-ttu-id="33a92-110">Internet Explorer 10 і новіших версій</span><span class="sxs-lookup"><span data-stu-id="33a92-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="33a92-111">Інші браузери, як-от Google Chrome і Mozilla Firefox, не підтримуються.</span><span class="sxs-lookup"><span data-stu-id="33a92-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="33a92-112">Ваша організація може підключитися до кінцевої точки в Azure, яка є **\* .blob.core.windows.net** (символ узагальнення представляє унікальний ідентифікатор завдання експорту).</span><span class="sxs-lookup"><span data-stu-id="33a92-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="33a92-113">У Центрі безпеки та відповідності Microsoft 365 вам призначається роль &amp; "Експорт".</span><span class="sxs-lookup"><span data-stu-id="33a92-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="33a92-114">За замовчуванням цю роль призначають лише групі ролей Диспетчера витребування електронної інформації.</span><span class="sxs-lookup"><span data-stu-id="33a92-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="33a92-115">Докладні відомості див. в розділі Призначення [дозволів на витребування електронної даних.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)</span><span class="sxs-lookup"><span data-stu-id="33a92-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="33a92-116">Докладні відомості див. [визятого нарада](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)в експорт результатів пошуку вмісту.</span><span class="sxs-lookup"><span data-stu-id="33a92-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="33a92-117">Якщо ви експортуєте понад 100K поштових скриньок, завантажте результати експорту за допомогою наведеної нижче оболонки PowerShell: експорт результатів із понад [100K-поштових скриньок.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)</span><span class="sxs-lookup"><span data-stu-id="33a92-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>