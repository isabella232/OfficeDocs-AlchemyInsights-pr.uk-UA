---
title: засіб експорту Витребування eDiscovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277932"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Не вдається інсталювати або запустити засіб експорту Витребування eDiscovery?

Якщо не вдається інсталювати або запустити засіб експорту Витребування електронної інформації для завантаження результатів пошуку, перевірте наведені нижче дії.
  
- Комп'ютер, який використовується, задовольняє ці передумови:

  - 32 або 64-розрядні версії ОС Windows 7 і новіші версії

  - Microsoft .NET Framework 4.7

  - Підтримуваний браузер:

  - Microsoft EDGE

    Або

  - Internet Explorer 10 і пізніші версії

    Інші браузери, як-от Google Chrome і Mozilla Firefox, не підтримуються.

- Ваша організація може підключитися до кінцевої точки в лазур, що є ** \* . BLOB.Core.Windows.net** (символ узагальнення – унікальний ідентифікатор для завдання для експорту).

- Ви призначили роль експорту в &amp; центрі відповідності системи безпеки Microsoft 365. За замовчуванням ця роль призначається лише рольовій групі "Диспетчер виявлення". Дивіться [призначення дозволів на відкриття електронної](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)інформації.

Докладні відомості наведено в статті [Експорт результатів пошуку вмісту](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Якщо ви експортуєте понад 100K поштові скриньки, вам доведеться використовувати наведені нижче PowerShell, щоб завантажити результати експорту:  [Експорт результатів із понад 100K поштових скриньок](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).