---
title: Інструкції з приховання та відображення групи зі списку адрес
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
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926266"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Приховання Microsoft 365 зі списку адрес (GAL)

Щоб приховати групу Microsoft 365 в списках адрес (GAL) клієнтів Exchange (наприклад, Outlook або OWA), використовуйте в оболонці EXO таку команду:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Щоб приховати групу Microsoft 365 від відображення Exchange клієнтів, скористайтеся такою командою в оболонці EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

