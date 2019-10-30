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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768962"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>Сховати групу Office 365 зі списку адрес (GAL)

Щоб приховати групу Office 365 зі списків адрес (GAL) Exchange-клієнтів (наприклад, Outlook або OWA), скористайтеся такою командою в EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Щоб приховати групу Office 365, видимі для Exchange клієнтів, скористайтеся такою командою в EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

