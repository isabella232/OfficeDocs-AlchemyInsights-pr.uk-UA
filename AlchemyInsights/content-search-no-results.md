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
# <a name="no-results-from-content-searchexports"></a>Результати пошуку та експорту вмісту відсутні

Проблеми з пошуком і експортом вмісту не повертають жодних даних, можливо, пов'язано з певним фільтром безпеки відповідності, який назначив певний адміністратор і не повідомив його всім адміністраторам.

Щоб вирішити цю проблему, перевірте, чи є фільтри безпеки відповідності, які можуть призвести до такої проблеми:
1. Підключення до Центру безпеки та відповідності PowerShell
2. Виконайте такі командлети:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org