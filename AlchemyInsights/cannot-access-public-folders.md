---
title: Не вдається отримати доступ до спільних папок
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
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819533"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не може підключитися до спільних папок

Якщо доступ до спільної папки не працює для деяких користувачів, спробуйте зробити ось що:

Підключіться до EXO PowerShell і настройте параметр DefaultPublicFolderMailbox в обліковому записі користувача, який відповідає параметру робочого облікового запису користувача.

Приклад.

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Зачекайте принаймні годину, доки зміни наберуть сили.

Якщо проблема не зсунеться, виконайте [цю процедуру,](https://aka.ms/pfcte) щоб усунути проблеми доступу до спільної папки за допомогою Outlook.
 
**Щоб визначити, які користувачі мають доступ до спільних папок, за допомогою Outlook, див.**

1.  Використання Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true або $false  
      
    $true: надання користувачам доступу до спільних папок в Outlook  
      
    $false. Заборона доступу користувачів до спільних папок в Outlook. ; ; ;Це значення за замовчуванням.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Примітка** Ця процедура може керувати підключеннями лише з класичною програмою Outlook для клієнтів Windows. Користувач може і надалі отримувати доступ до спільних папок за допомогою OWA або Outlook для Mac.
 
Докладні відомості див. в статтях Про підтримку керованих підключень до [спільних папок в Outlook.](https://aka.ms/controlpf)