---
title: Відновлення видаленої спільної папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063778"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="77e73-102">Відновлення видаленої спільної папки</span><span class="sxs-lookup"><span data-stu-id="77e73-102">Restore a deleted public folder</span></span>

<span data-ttu-id="77e73-103">**Щоб відновити видалені елементи з спільної папки**:</span><span class="sxs-lookup"><span data-stu-id="77e73-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="77e73-104">[Не можна відновити видалені елементи з не електронної пошти спільної папки в Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="77e73-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="77e73-105">**Щоб відновити видалену загальнопублічну папку (будь-який тип)**:</span><span class="sxs-lookup"><span data-stu-id="77e73-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="77e73-106">Будь ласка, використовуйте наступні EXO PowerShell команди:</span><span class="sxs-lookup"><span data-stu-id="77e73-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="77e73-107">Синтаксис:</span><span class="sxs-lookup"><span data-stu-id="77e73-107">Syntax:</span></span>

    ><span data-ttu-id="77e73-108">$pf = Get-Публітека \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-повторюється |? {$_. Назва-EQ "\<name_of_deleted_public_Folder"}; Set-Публітека $pf. \<шлях до ідентифікації, де буде відновлено папку></span><span class="sxs-lookup"><span data-stu-id="77e73-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="77e73-109">Приклад: Наступна команда відновить Subfolder1 і помістіть його до \Parent1:</span><span class="sxs-lookup"><span data-stu-id="77e73-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="77e73-110">$pf = Get-Публітека \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-повторюється |? {$_. Назва-EQ "Subfolder1"}; Set-Публіцитека $pf. шлях до посвідчення \ parent1</span><span class="sxs-lookup"><span data-stu-id="77e73-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="77e73-111">Щоб отримати додаткові відомості, перегляньте цю [папку](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="77e73-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
