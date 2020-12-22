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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727244"
---
# <a name="no-results-returned-during-content-searchexport"></a>Під час пошуку або експорту вмісту не повернуто жодних результатів

Якщо виникають проблеми з такими сценаріями eDiscovery:

- Функція пошуку або експорту не повертає дані або несподівані дані
- Пошук або експорт електронного розкриття інформації

Це може бути пов'язано з певними фільтрами безпеки, які інсталювалися за певним адміністратором, і не були повідомлені всім адміністраторам.

Щоб вирішити цю проблему, перевірте, чи є які-небудь фільтри безпеки відповідності, які можуть викликати ці проблеми.

1. Підключення до центру безпеки та відповідності PowerShell
2. Виконайте такі командлетів:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Додаткові відомості про фільтри безпеки відповідності наведено в статті [фільтрування дозволів для пошуку вмісту](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
