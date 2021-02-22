---
title: Приховання спільних папок
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315444"
---
# <a name="hide-public-folders"></a>Приховання спільних папок

**Щоб приховати все дерево загальнодоступної папки**, зробіть ось що.

Виконайте кроки, описані в [цій](https://aka.ms/ControlPF) статті, щоб приховати всю ялинку загальнодоступної папки з вибіркових або всіх користувачів.

**Щоб приховати певну спільну папку,** виконайте наведені нижче дії.

1. Додавання дозволів для користувачів, яким потрібно отримати доступ до спільної папки

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Видаліть користувача **за замовчуванням** зі списку **дозволів** .

    `Remove-PublicFolderClientPermission \test1 -User Default`
