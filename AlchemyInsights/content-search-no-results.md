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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058023"
---
# <a name="no-results-from-content-searchexports"></a>Результати пошуку та експорту вмісту відсутні

Проблеми з пошуком і експортом вмісту не повертають жодних даних, можливо, пов'язано з певним фільтром безпеки відповідності, який назначив певний адміністратор і не повідомив його всім адміністраторам.

Щоб вирішити цю проблему, перевірте, чи є фільтри безпеки відповідності, які можуть призвести до такої проблеми:
1. Підключення до Центру безпеки та відповідності PowerShell
2. Виконайте такі командлети:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org