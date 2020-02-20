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
# <a name="restore-a-deleted-public-folder"></a>Відновлення видаленої спільної папки

**Щоб відновити видалені елементи з спільної папки**:

- [Не можна відновити видалені елементи з не електронної пошти спільної папки в Outlook 2016](https://aka.ms/pfrec).
 
**Щоб відновити видалену загальнопублічну папку (будь-який тип)**: 

- Будь ласка, використовуйте наступні EXO PowerShell команди:

    Синтаксис:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Приклад: Наступна команда відновить Subfolder1 і помістіть його до \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Щоб отримати додаткові відомості, перегляньте цю [папку](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
