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
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158549"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="9081e-102">Відновлення видаленої спільної папки</span><span class="sxs-lookup"><span data-stu-id="9081e-102">Restore a deleted public folder</span></span>

<span data-ttu-id="9081e-103">**Щоб відновити видалені елементи з спільної папки**:</span><span class="sxs-lookup"><span data-stu-id="9081e-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="9081e-104">[Не можна відновити видалені елементи з не електронної пошти спільної папки в Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="9081e-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="9081e-105">**Щоб відновити видалену загальнопублічну папку (будь-який тип)**:</span><span class="sxs-lookup"><span data-stu-id="9081e-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="9081e-106">Будь ласка, використовуйте наступні EXO PowerShell команди:</span><span class="sxs-lookup"><span data-stu-id="9081e-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="9081e-107">Синтаксис:</span><span class="sxs-lookup"><span data-stu-id="9081e-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="9081e-108">Приклад: Наступна команда відновить Subfolder1 і помістіть його до \Parent1:</span><span class="sxs-lookup"><span data-stu-id="9081e-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="9081e-109">Щоб отримати додаткові відомості, перегляньте цю [папку](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="9081e-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
