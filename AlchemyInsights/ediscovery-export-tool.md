---
title: Засіб експорту витребування електронної пошти
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814609"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не вдається інсталювати або запустити засіб експорту витребування електронної даних?

Якщо не вдається інсталювати або запустити засіб експорту витребування електронної даних, щоб завантажити результати пошуку, перевірте таке:
  
- Використовується комп'ютер, відповідає таким вимогам:

  - 32- або 64-розрядна версія Windows 7 і пізніших версій

  - Microsoft .NET Framework 4.7

  - Підтримуваний браузер:

  - Microsoft Edge

    Або

  - Internet Explorer 10 і новіших версій

    Інші браузери, як-от Google Chrome і Mozilla Firefox, не підтримуються.

- Ваша організація може підключитися до кінцевої точки в Azure, яка є **\* .blob.core.windows.net** (символ узагальнення представляє унікальний ідентифікатор завдання експорту).

- У Центрі безпеки та відповідності Microsoft 365 вам призначається роль &amp; "Експорт". За замовчуванням цю роль призначають лише групі ролей Диспетчера витребування електронної інформації. Докладні відомості див. в розділі Призначення [дозволів на витребування електронної даних.](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)

Докладні відомості див. [визятого нарада](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)в експорт результатів пошуку вмісту.

Якщо ви експортуєте понад 100K поштових скриньок, завантажте результати експорту за допомогою наведеної нижче оболонки PowerShell: експорт результатів із понад [100K-поштових скриньок.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)