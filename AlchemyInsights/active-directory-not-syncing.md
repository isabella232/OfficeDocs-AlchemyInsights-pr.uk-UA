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
ms.openlocfilehash: 4bfbe6b2dd9a2112f0cb7af0d6e7a46693bc70680895fd674ddb0332b7071797
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53937122"
---
# <a name="active-directory-not-syncing"></a>Служба Active Directory не синхронізується

Якщо ви отримуєте помилки синхронізації, наприклад "нещодавня синхронізація" або помітили стан синхронізації служби каталогів на порталі адміністрування Office промовить фраза "Востаннє синхронізовано більше трьох днів тому", можливо, AADConnect має неправильні параметри або недостатньо дозволів на синхронізацію.  

Якщо повторно інсталювати AADConnect за допомогою швидких настройок, проблему можна швидко вирішити.

1. [Завантажте найновішу версію AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Дотримуйтеся вказівок щодо швидкого інсталяції](/azure/active-directory/hybrid/how-to-connect-install-express).

У Windows Server 2012 або пізніших версіях має бути інстальовано Azure AD Connect. Цей сервер має бути підключений до домену та може бути контролером домену або сервером-учасником. Повний список вимог і попередніх Підключення Azure AD див. в передумови [для Azure AD Підключення](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).

Докладні відомості про облікові записи служб AADConnect див. в розділі [Azure AD Підключення: облікові записи та дозволи.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)
