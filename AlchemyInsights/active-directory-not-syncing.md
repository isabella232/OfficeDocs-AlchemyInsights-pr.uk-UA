---
title: Active Directory не синхронізується
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265277"
---
# <a name="active-directory-not-syncing"></a>Active Directory не синхронізується

Якщо ви отримуєте помилки синхронізації, наприклад, "немає останньої синхронізації" або зверніть увагу на стан синхронізації каталогів на порталі Office Admin говориться, "Остання синхронізація більше 3 днів тому", може бути, що AADConnect має неправильні параметри або недостатньо дозволи на виконання синхронізації.  

Повторна інсталяція AADConnect за допомогою Експрес-настройок може швидко вирішити проблему:

1. [Завантажити останню версію AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Дотримуйтеся вказівок для Експрес-інсталяції](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Щоб отримати додаткові відомості про AADConnect служби облікових записів, див [AZURE AD-підключення: облікові записи та дозволи](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
