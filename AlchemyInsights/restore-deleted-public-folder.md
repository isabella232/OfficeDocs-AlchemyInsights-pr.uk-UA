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
# <a name="restore-a-deleted-public-folder"></a>Відновлення видаленої спільної папки

**Щоб відновити видалені елементи з спільної папки**:

- [Не можна відновити видалені елементи з не електронної пошти спільної папки в Outlook 2016](https://aka.ms/pfrec).
 
**Щоб відновити видалену загальнопублічну папку (будь-який тип)**: 

- Будь ласка, використовуйте наступні EXO PowerShell команди:

    Синтаксис:

    >$pf = Get-Публітека \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-повторюється |? {$_. Назва-EQ "\<name_of_deleted_public_Folder"}; Set-Публітека $pf. \<шлях до ідентифікації, де буде відновлено папку>

    Приклад: Наступна команда відновить Subfolder1 і помістіть його до \Parent1:

    >$pf = Get-Публітека \ NON_IPM_SUBTREE \ DUMPSTER_ROOT-повторюється |? {$_. Назва-EQ "Subfolder1"}; Set-Публіцитека $pf. шлях до посвідчення \ parent1

Щоб отримати додаткові відомості, перегляньте цю [папку](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
