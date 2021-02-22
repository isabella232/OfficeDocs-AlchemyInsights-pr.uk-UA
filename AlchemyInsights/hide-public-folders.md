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
# <a name="hide-public-folders"></a><span data-ttu-id="106db-102">Приховання спільних папок</span><span class="sxs-lookup"><span data-stu-id="106db-102">Hide public folders</span></span>

<span data-ttu-id="106db-103">**Щоб приховати все дерево загальнодоступної папки**, зробіть ось що.</span><span class="sxs-lookup"><span data-stu-id="106db-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="106db-104">Виконайте кроки, описані в [цій](https://aka.ms/ControlPF) статті, щоб приховати всю ялинку загальнодоступної папки з вибіркових або всіх користувачів.</span><span class="sxs-lookup"><span data-stu-id="106db-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="106db-105">**Щоб приховати певну спільну папку,** виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="106db-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="106db-106">Додавання дозволів для користувачів, яким потрібно отримати доступ до спільної папки</span><span class="sxs-lookup"><span data-stu-id="106db-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="106db-107">Видаліть користувача **за замовчуванням** зі списку **дозволів** .</span><span class="sxs-lookup"><span data-stu-id="106db-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
