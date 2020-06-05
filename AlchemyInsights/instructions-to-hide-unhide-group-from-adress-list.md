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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580030"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Приховання групи Microsoft 365 зі списку адрес (GAL)

Щоб приховати групу Microsoft 365 зі списків адрес (GAL) для клієнтів Exchange (наприклад, Outlook або OWA), скористайтеся такою командою в EXO оболонці:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Щоб приховати групу Microsoft 365, видимі для Exchange клієнтів, скористайтеся такою командою в EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

