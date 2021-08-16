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
ms.openlocfilehash: a5acd322186f8f4b7734f8541877a642a553288e10b3c122e4f276b9bb611308
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989000"
---
# <a name="auditing-in-microsoft-365"></a>Аудит у Microsoft 365

Ось кілька речей, які слід знати про аудит у Microsoft 365:

1. Exchange дії адміністратора перевіряються за замовчуванням.
1. Ми активуємо аудит поштових скриньок за замовчуванням для всіх користувачів. Щоб дізнатися більше про це, клацніть [тут](https://techcommunity.microsoft.com/t5/Security-Privacy-and-Compliance/Exchange-Mailbox-Auditing-will-be-enabled-by-default/ba-p/215171). Доки ви не бажаєте вручну ввімкнути цю функцію для одного користувача або всієї організації, натисніть нижче кнопку Увімкнути аудит поштових скриньок.
1. Microsoft 365 Поштові скриньки групи та поштові скриньки спільних папок не підтримують журналювання аудиту.
1. Щоб SharePoint або OneDrive, додаткові параметри, необхідні для аудиту, не потрібно. Щоб дізнатися, які дії перевірено, див. такі дії:
    1. [Дії з файлами](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#file-and-page-activities)
    1. [Дії з папками](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    1. [Дії з надання спільного доступу та доступ до даних](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities).
1. Список усіх від перевірених дій за службами див. в цьому [списку.](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#audited-activities)
