---
title: Результати пошуку вмісту відсутні
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816869"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="334b2-102">Результати пошуку та експорту вмісту відсутні</span><span class="sxs-lookup"><span data-stu-id="334b2-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="334b2-103">Проблеми з пошуком і експортом вмісту не повертають жодних даних, можливо, пов'язано з певним фільтром безпеки відповідності, який назначив певний адміністратор і не повідомив його всім адміністраторам.</span><span class="sxs-lookup"><span data-stu-id="334b2-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="334b2-104">Щоб вирішити цю проблему, перевірте, чи є фільтри безпеки відповідності, які можуть призвести до такої проблеми:</span><span class="sxs-lookup"><span data-stu-id="334b2-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="334b2-105">Підключення до Центру безпеки та відповідності PowerShell</span><span class="sxs-lookup"><span data-stu-id="334b2-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="334b2-106">Виконайте такі командлети:</span><span class="sxs-lookup"><span data-stu-id="334b2-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="334b2-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="334b2-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="334b2-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="334b2-108">Get-ComplianceSecurityFilter -Organization $org</span></span>