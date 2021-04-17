---
title: Служба Active Directory не синхронізується
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822872"
---
# <a name="active-directory-not-syncing"></a>Служба Active Directory не синхронізується

Якщо ви отримуєте помилки синхронізації, наприклад "нещодавня синхронізація" або помітили стан синхронізації служби каталогів на порталі адміністрування Office, промовляється "Востаннє синхронізовано більше трьох днів тому", можливо, AADConnect має неправильні параметри або недостатньо дозволів на синхронізацію.  

Якщо повторно інсталювати AADConnect за допомогою швидких настройок, проблему можна швидко вирішити.

1. [Завантажте найновішу версію AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Дотримуйтеся вказівок щодо швидкого інсталяції](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Докладні відомості про облікові записи служб AADConnect див. в розділі [Azure AD Connect: облікові записи та дозволи.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
