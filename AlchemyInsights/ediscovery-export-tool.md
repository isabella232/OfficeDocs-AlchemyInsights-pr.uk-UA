---
title: засіб експорту Витребування eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277932"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="d1e38-102">Не вдається інсталювати або запустити засіб експорту Витребування eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="d1e38-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="d1e38-103">Якщо не вдається інсталювати або запустити засіб експорту Витребування електронної інформації для завантаження результатів пошуку, перевірте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="d1e38-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="d1e38-104">Комп'ютер, який використовується, задовольняє ці передумови:</span><span class="sxs-lookup"><span data-stu-id="d1e38-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="d1e38-105">32 або 64-розрядні версії ОС Windows 7 і новіші версії</span><span class="sxs-lookup"><span data-stu-id="d1e38-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="d1e38-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="d1e38-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="d1e38-107">Підтримуваний браузер:</span><span class="sxs-lookup"><span data-stu-id="d1e38-107">A supported browser:</span></span>

  - <span data-ttu-id="d1e38-108">Microsoft EDGE</span><span class="sxs-lookup"><span data-stu-id="d1e38-108">Microsoft Edge</span></span>

    <span data-ttu-id="d1e38-109">Або</span><span class="sxs-lookup"><span data-stu-id="d1e38-109">Or</span></span>

  - <span data-ttu-id="d1e38-110">Internet Explorer 10 і пізніші версії</span><span class="sxs-lookup"><span data-stu-id="d1e38-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="d1e38-111">Інші браузери, як-от Google Chrome і Mozilla Firefox, не підтримуються.</span><span class="sxs-lookup"><span data-stu-id="d1e38-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="d1e38-112">Ваша організація може підключитися до кінцевої точки в лазур, що є \*\* \* . BLOB.Core.Windows.net\*\* (символ узагальнення – унікальний ідентифікатор для завдання для експорту).</span><span class="sxs-lookup"><span data-stu-id="d1e38-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="d1e38-113">Ви призначили роль експорту в &amp; центрі відповідності системи безпеки Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d1e38-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="d1e38-114">За замовчуванням ця роль призначається лише рольовій групі "Диспетчер виявлення".</span><span class="sxs-lookup"><span data-stu-id="d1e38-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="d1e38-115">Дивіться [призначення дозволів на відкриття електронної](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)інформації.</span><span class="sxs-lookup"><span data-stu-id="d1e38-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="d1e38-116">Докладні відомості наведено в статті [Експорт результатів пошуку вмісту](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="d1e38-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="d1e38-117">Якщо ви експортуєте понад 100K поштові скриньки, вам доведеться використовувати наведені нижче PowerShell, щоб завантажити результати експорту:  [Експорт результатів із понад 100K поштових скриньок](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="d1e38-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>