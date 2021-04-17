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
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831899"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Приховання групи Microsoft 365 зі списку адрес (GAL)

Щоб приховати групу Microsoft 365 у списках адрес (GAL) клієнтів Exchange (наприклад, Outlook або OWA), скористайтеся такою командою в оболонці EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Щоб приховати групу Microsoft 365 від видимості для клієнтів Exchange, скористайтеся такою командою в оболонці EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

