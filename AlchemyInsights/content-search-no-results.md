---
title: Результати пошуку вмісту не відображаються
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680668"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="4205c-102">Без результатів пошуку та експорту вмісту</span><span class="sxs-lookup"><span data-stu-id="4205c-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="4205c-103">Проблеми з пошуком або експортом вмісту не повертаються будь-які дані можуть бути викликані певним адміністратором системи безпеки, установлену для певного адміністратора, а не спілкуватися з усіма адміністраторами.</span><span class="sxs-lookup"><span data-stu-id="4205c-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="4205c-104">Щоб вирішити цю проблему, перевірте, чи існують будь-які фільтри безпеки відповідності, які можуть бути причиною цього:</span><span class="sxs-lookup"><span data-stu-id="4205c-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="4205c-105">Підключення до центру безпеки та відповідності PowerShell</span><span class="sxs-lookup"><span data-stu-id="4205c-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="4205c-106">Виконайте такі командлетів:</span><span class="sxs-lookup"><span data-stu-id="4205c-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="4205c-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="4205c-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="4205c-108">Get-ComplianceSecurityFilter-організація $org</span><span class="sxs-lookup"><span data-stu-id="4205c-108">Get-ComplianceSecurityFilter -Organization $org</span></span>