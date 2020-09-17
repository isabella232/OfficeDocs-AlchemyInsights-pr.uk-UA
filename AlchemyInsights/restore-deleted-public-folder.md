---
title: Відновлення видаленої загальнодоступної папки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774552"
---
# <a name="restore-a-deleted-public-folder"></a>Відновлення видаленої загальнодоступної папки

**Щоб відновити видалені елементи зі спільної папки,** виконайте наведені нижче дії.

- Дізнайтеся, [що не можна відновити видалені повідомлення з загальнодоступної папки в програмі Outlook 2016](https://aka.ms/pfrec).
 
**Щоб відновити видалену спільну папку (будь-якого типу), виконайте такі**дії: 

- Скористайтеся наступною командою EXO PowerShell:

    Синтаксис

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Приклад: наведена нижче команда відновить Subfolder1 та розмістіть його в розділі \Pare1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Щоб отримати докладні відомості, Дізнайтеся, [як відновити видалену спільну папку](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
