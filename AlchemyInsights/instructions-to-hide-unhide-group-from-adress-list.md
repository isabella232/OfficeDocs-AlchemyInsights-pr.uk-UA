---
title: Інструкції з приховання або відображення групи зі списку адрес
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
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663030"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Приховання групи Microsoft 365 зі списку адрес (GAL)

Щоб приховати групу Microsoft 365 зі списків адрес (GAL) клієнтів Exchange (наприклад, Outlook або OWA), скористайтеся наведенною нижче командою в програмі EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Щоб приховати групу Microsoft 365 від видимості для Exchange для клієнтів, скористайтеся наведенною нижче командою в програмі EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

