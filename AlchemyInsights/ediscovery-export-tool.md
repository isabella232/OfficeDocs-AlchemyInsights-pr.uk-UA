---
title: Витребування електронної інформації для експорту
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/3/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 5a54344d43d16c77d440768aa1c87489edf10ca0
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736346"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не вдається інсталювати або запустити засіб експортування необхідної інформації?

Якщо ви не можете встановити або запустити засіб експортування електронної інформації Office 365 для завантаження результатів пошуку, перевірте такі речі:
  
- Комп'ютер, який ви використовуєте, відповідає цим попередньо реквізитам:

  - 32-або 64-розрядних версій ОС Windows 7 і пізніших версій

  - Microsoft .NET Framework 4,7

  - Підтримуваний браузер:

  - Microsoft EDGE

    Або

  - Internet Explorer 10 і пізніших версій

    Інші браузери, такі як Google Chrome і Mozilla Firefox, не підтримуються.

- Ваша організація може підключатися до кінцевої точки в Azure, яка є ** \*. BLOB.Core.Windows.net** (у підстановці є унікальним ідентифікатором для завдання експорту).

- Ви признаєтеся ролі експорту в центрі забезпечення дотримання безпеки &amp; Office 365. За промовчанням ця роль призначається лише для рольової групи «Витребування менеджера». Див [.](https://docs.microsoft.com/office365/securitycompliance/assign-ediscovery-permissions)

Докладніші відомості наведено в [результатах пошуку в експортному вмісті](https://docs.microsoft.com/office365/securitycompliance/export-search-results).
  