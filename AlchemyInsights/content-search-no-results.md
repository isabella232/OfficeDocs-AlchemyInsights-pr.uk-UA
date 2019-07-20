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
# <a name="no-results-from-content-searchexports"></a>Немає результатів від вмісту пошуку/експорт

Проблеми з контентом пошук/експорту не повертаються дані, може бути пов'язано з певних дотримання безпеки фільтр, який був налаштування конкретних адміністратора і не інформувати про це всіх адміністраторів.

Щоб усунути помилку, перевірте, якщо є будь-які фільтри дотримання безпеки, які можуть викликати це:
1. Підключитися до безпеки і відповідності центр Powershell
2. Запустіть наступну commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-організація $org