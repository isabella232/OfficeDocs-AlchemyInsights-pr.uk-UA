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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943396"
---
# <a name="restore-a-deleted-public-folder"></a>Відновлення видаленої спільної папки

**Щоб відновити видалені елементи зі спільної папки:**

- Докладні [відомості див. в](https://aka.ms/pfrec)цій Outlook 2016 .
 
**Щоб відновити видалену спільну папку (будь-якого типу):** 

- Виконайте таку команду EXO PowerShell:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Приклад. Наведена нижче команда відновить вкладену доріжку1 і розмістить її в розділі \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Докладні [відомості див. в папці](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) Відновлення видаленої спільної папки.
