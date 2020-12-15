---
title: Під час пошуку або експорту вмісту не повернуто жодних результатів
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680332"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="9113f-102">Під час пошуку або експорту вмісту не повернуто жодних результатів</span><span class="sxs-lookup"><span data-stu-id="9113f-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="9113f-103">Якщо виникають проблеми з такими сценаріями eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="9113f-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="9113f-104">Функція пошуку або експорту не повертає дані або несподівані дані</span><span class="sxs-lookup"><span data-stu-id="9113f-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="9113f-105">Пошук або експорт електронного розкриття інформації</span><span class="sxs-lookup"><span data-stu-id="9113f-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="9113f-106">Це може бути викликано через певні фільтри безпеки, які були встановлені певним адміністратором, і не були повідомлені всім адміністраторам.</span><span class="sxs-lookup"><span data-stu-id="9113f-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="9113f-107">Щоб вирішити цю проблему, перевірте, чи є які-небудь фільтри безпеки відповідності, які можуть викликати ці проблеми.</span><span class="sxs-lookup"><span data-stu-id="9113f-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="9113f-108">Підключення до центру безпеки та відповідності PowerShell</span><span class="sxs-lookup"><span data-stu-id="9113f-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="9113f-109">Виконайте такі командлетів:</span><span class="sxs-lookup"><span data-stu-id="9113f-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="9113f-110">Додаткові відомості про фільтри безпеки відповідності наведено в статті [фільтрування дозволів для пошуку вмісту](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="9113f-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
