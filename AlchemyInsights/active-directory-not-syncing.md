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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314225"
---
# <a name="active-directory-not-syncing"></a>Служба Active Directory не синхронізується

Якщо ви отримуєте помилки синхронізації, наприклад "нещодавня синхронізація", або помітите стан синхронізації служби каталогів на порталі адміністрування Office промовить фраза "Last synced more 3 days ago" (Востаннє синхронізовано більше трьох днів тому), імовірно, AADConnect має неправильні параметри або недостатньо дозволів на синхронізацію.  

Якщо повторно інсталювати AADConnect за допомогою швидких настройок, проблему можна швидко вирішити.

1. [Завантажте найновішу версію AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Дотримуйтеся вказівок щодо швидкого інсталяції](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

У Windows Server 2012 або пізніших версіях має бути інстальовано Azure AD Connect. Цей сервер має бути підключений до домену та може бути контролером домену або сервером-учасником. Повний список вимог і попередніх Підключення Azure AD див. в попередніх версіях [Azure AD Підключення](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Докладні відомості про облікові записи служб AADConnect див. в розділі [Azure AD Підключення: облікові записи та дозволи.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
