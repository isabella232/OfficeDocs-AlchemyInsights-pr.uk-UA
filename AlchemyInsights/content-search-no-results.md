---
title: Вміст не результати пошуку
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800682"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="cd107-102">Немає результатів від вмісту пошуку/експорт</span><span class="sxs-lookup"><span data-stu-id="cd107-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="cd107-103">Проблеми з контентом пошук/експорту не повертаються дані, може бути пов'язано з певних дотримання безпеки фільтр, який був налаштування конкретних адміністратора і не інформувати про це всіх адміністраторів.</span><span class="sxs-lookup"><span data-stu-id="cd107-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="cd107-104">Щоб усунути помилку, перевірте, якщо є будь-які фільтри дотримання безпеки, які можуть викликати це:</span><span class="sxs-lookup"><span data-stu-id="cd107-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="cd107-105">Підключитися до безпеки і відповідності центр Powershell</span><span class="sxs-lookup"><span data-stu-id="cd107-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="cd107-106">Запустіть наступну commandlets:</span><span class="sxs-lookup"><span data-stu-id="cd107-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="cd107-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="cd107-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="cd107-108">Get-ComplianceSecurityFilter-організація $org</span><span class="sxs-lookup"><span data-stu-id="cd107-108">Get-ComplianceSecurityFilter -Organization $org</span></span>