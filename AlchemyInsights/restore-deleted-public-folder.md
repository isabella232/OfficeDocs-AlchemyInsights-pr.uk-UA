---
title: Відновлення видаленої спільної папки
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
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809460"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="509ec-102">Відновлення видаленої спільної папки</span><span class="sxs-lookup"><span data-stu-id="509ec-102">Restore a deleted public folder</span></span>

<span data-ttu-id="509ec-103">**Щоб відновити видалені елементи зі спільної папки:**</span><span class="sxs-lookup"><span data-stu-id="509ec-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="509ec-104">Див. [3. В Outlook 2016](https://aka.ms/pfrec)не можна відновити видалені елементи зі спільної папки, яка не надається електронною поштою.</span><span class="sxs-lookup"><span data-stu-id="509ec-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="509ec-105">**Щоб відновити видалену спільну папку (будь-якого типу):**</span><span class="sxs-lookup"><span data-stu-id="509ec-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="509ec-106">Виконайте таку команду EXO PowerShell:</span><span class="sxs-lookup"><span data-stu-id="509ec-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="509ec-107">Синтаксис:</span><span class="sxs-lookup"><span data-stu-id="509ec-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="509ec-108">Приклад. Наведена нижче команда відновить вкладену доріжку1 і розмістить її в розділі \Parent1:</span><span class="sxs-lookup"><span data-stu-id="509ec-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="509ec-109">Докладні [відомості див. в папці](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Відновлення видаленої спільної папки.</span><span class="sxs-lookup"><span data-stu-id="509ec-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
