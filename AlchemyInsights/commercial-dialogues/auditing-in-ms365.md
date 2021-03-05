---
title: Аудит у Microsoft 365
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
- "3100005"
- "7327"
ms.openlocfilehash: c07981bfae40d74deb1a2f143ce51da69b51a69f
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483415"
---
# <a name="auditing-in-microsoft-365"></a>Аудит у Microsoft 365

Нижче наведено кілька порад про відстеження в Microsoft 365.

1. Дії з адміністрування Exchange перевіряються за замовчуванням.
1. Ми перебуваємо в процесі ввімкнення аудиту поштової скриньки за замовчуванням для всіх користувачів. Щоб дізнатися більше про це, натисніть [тут](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171). Якщо потрібно, щоб вказівки вручну могли ввімкнути його для однієї особи або всієї організації, натисніть кнопку увімкнути аудит поштової скриньки нижче.
1. Поштові скриньки груп Microsoft 365 і поштові скриньки спільних папок не підтримують журналювання аудиту.
1. Для служби SharePoint або OneDrive немає додаткової конфігурації, необхідної для ввімкнення аудиту. Щоб дізнатися, які дії відстежуватиметься, перегляньте:
    1. [Дії з файлами](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [Дії з папками](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [Надання спільного доступу та дій Access](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).
1. Щоб переглянути список усіх перевірених дій за допомогою служби, ознайомтеся з діями, що [перевіряються](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities).
