---
title: Під час пошуку та експорту вмісту не повертаються жодні результати
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
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101287"
---
# <a name="no-results-returned-during-content-searchexport"></a>Під час пошуку та експорту вмісту не повертаються жодні результати

Якщо виникають проблеми з такими сценаріями витребування електронної пошти:

- Під час пошуку та експорту вмісту не повертаються дані або неочікувані дані
- Помилка пошуку витребування електронної пошти або експорту

Це може бути через певні фільтри безпеки відповідності, які назначає певний адміністратор, і його повідомили не всі адміністратори.

Щоб вирішити цю проблему, перевірте, чи є фільтри безпеки відповідності, які можуть призвести до таких проблем:

1. Підключення до Центру безпеки та відповідності PowerShell
2. Виконайте такі командлети:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Докладні відомості про фільтри безпеки відповідності див. в розділі [Фільтрування дозволів для пошуку вмісту.](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
