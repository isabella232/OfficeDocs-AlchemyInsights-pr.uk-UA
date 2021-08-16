---
title: Керування доступом до спільних папок за допомогою Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 1386b97f804e63455094abf64b9d9e2541d57dafa36535813b0d7689e0ce2966
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54032579"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Керування доступом до спільних папок за допомогою Outlook

Щоб визначити, які користувачі мають доступ до спільних папок, за допомогою Outlook:

1. Використання `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true. Надання користувачам доступу до спільних папок у Outlook  
$false. Заборона доступу користувачів до спільних папок у Outlook. ; ; ;Це значення за замовчуванням.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Примітка. Ця процедура може керувати підключеннями лише з Outlook пк для Windows клієнтів. Користувачі можуть і надалі отримувати доступ до спільних папок за допомогою OWA або Outlook для Mac.

Докладні відомості див. в [статтях Керовані](https://aka.ms/controlpf) підключення до спільних папок Outlook докладні відомості.
