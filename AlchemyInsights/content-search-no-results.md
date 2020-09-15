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
# <a name="no-results-from-content-searchexports"></a>Без результатів пошуку та експорту вмісту

Проблеми з пошуком або експортом вмісту не повертаються будь-які дані можуть бути викликані певним адміністратором системи безпеки, установлену для певного адміністратора, а не спілкуватися з усіма адміністраторами.

Щоб вирішити цю проблему, перевірте, чи існують будь-які фільтри безпеки відповідності, які можуть бути причиною цього:
1. Підключення до центру безпеки та відповідності PowerShell
2. Виконайте такі командлетів:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-організація $org