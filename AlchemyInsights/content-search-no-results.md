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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516800"
---
# <a name="no-results-from-content-searchexports"></a>Немає результатів від вмісту пошуку/експорт

Проблеми з контентом пошук/експорту не повертаються дані, може бути пов'язано з певних дотримання безпеки фільтр, який був налаштування конкретних адміністратора і не інформувати про це всіх адміністраторів.

Щоб усунути помилку, перевірте, якщо є будь-які фільтри дотримання безпеки, які можуть викликати це:
1. Підключитися до безпеки і відповідності центр Powershell
2. Запустіть наступну commandlets:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter-організація $org