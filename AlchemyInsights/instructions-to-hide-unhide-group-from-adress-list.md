---
title: Інструкції з приховування/відображення групи зі списку адрес
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908365"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Приховання групи Microsoft 365 зі списку адрес (GAL)

Щоб приховати групу Microsoft 365 зі списків адрес (GAL) для клієнтів Exchange (наприклад, Outlook або OWA), скористайтеся такою командою в EXO оболонці:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Щоб приховати групу Microsoft 365, видимі для Exchange клієнтів, скористайтеся такою командою в EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

