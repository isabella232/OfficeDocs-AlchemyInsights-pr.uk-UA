---
title: 1490 – усунення несправностей – eDiscovery – помилки
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277843"
---
# <a name="troubleshoot-content-search-errors"></a>Виправлення помилок пошуку вмісту

Під час експорту результатів пошуку виникають проблеми з пошуком вмісту або їх збої?

Наприклад, під час запуску пошуків відображається таке:

- Помилки CS008 або CS012

- Помилки на сервері/тайм-аут

- Сталася помилка програми

Або під час пошуку або експортування результатів із великої кількості поштових скриньок (понад 100 000 поштових скриньок) ви одержуєте помилки експорту?

Для цих типів помилок повторіть пошук розташувань вмісту, які не вдалося виконати. Перегляньте  [цю статтю](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) , щоб отримати докладніші відомості.

Якщо ви експортуєте понад 100K поштові скриньки, вам доведеться використовувати наведені нижче PowerShell, щоб завантажити результати експорту:  [Експорт результатів із понад 100K поштових скриньок](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).
