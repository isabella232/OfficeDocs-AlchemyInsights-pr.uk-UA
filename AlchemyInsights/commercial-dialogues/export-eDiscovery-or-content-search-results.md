---
title: Експорт результатів витребування електронної пошти та пошуку вмісту
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: de5d6f2bbf32ca1b7a0bbb9dd416fb19186d2e72ad57fbf25d9b55bd733fdc21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988208"
---
# <a name="export-ediscoverycontent-search-results"></a>Експорт результатів витребування електронної пошти та пошуку вмісту

Можливо, знадобиться експортувати результати пошуку у файл PST (з електронної пошти) або до власних Office документів (з SharePoint і OneDrive для бізнесу сайтів). У такому разі виконайте такі дії:

- Переконайтеся, що обліковому запису призначено необхідні дозволи на експорт. Докладні відомості див. в [описі призначення дозволів на витребування електронної інформації.](https://go.microsoft.com/fwlink/?linkid=2102406)
- Переконайтеся, що комп'ютер виконав [усі попередні умови.](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin) Підтримуються не всі браузери, наприклад Chrome.
- Щоб експортувати дані з поля пошуку вмісту, потрібно виконати таку команду: a. Перейдіть до Центру [безпеки & відповідності,](https://protection.office.com/contentsearch) клацніть **пошук**, а потім виберіть **Пошук вмісту**. На сторінці **"Пошук вмісту"** виберіть збережений пошук.
    b. В області Відомості в розділі Експорт **результатів до комп'ютера натисніть** кнопку Почати **експорт.** Якщо ви експортуєте понад 100K поштових скриньок, знадобиться скористатися PowerShell, щоб завантажити результати експорту. Докладні відомості див. в розділАх Експорт результатів із [понад 100K поштових скриньок.](https://go.microsoft.com/fwlink/?linkid=2143861)

Докладні відомості див. в [статтях Експорт результатів пошуку вмісту.](https://go.microsoft.com/fwlink/?linkid=2102118)