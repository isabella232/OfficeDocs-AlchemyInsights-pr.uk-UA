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
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996651"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook не вдається підключитися до спільних папок

Якщо доступ до спільної папки не працює для деяких користувачів, спробуйте зробити ось що:

Підключення exo PowerShell і настройте параметр DefaultPublicFolderMailbox в обліковому записі користувача, який відповідає параметру робочого облікового запису користувача.

Приклад.

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Зачекайте принаймні годину, доки зміни наберуть сили.

Якщо проблема залишиться, [](https://aka.ms/pfcte) виконайте цю процедуру, щоб усунути проблеми доступу до спільної папки за допомогою Outlook.
 
**Щоб визначити, які користувачі мають доступ до спільних папок, за допомогою Outlook:**

1.  Використання Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true або $false  
      
    $true. Надання користувачам доступу до спільних папок у Outlook  
      
    $false. Заборона доступу користувачів до спільних папок у Outlook. ; ; ;Це значення за замовчуванням.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Примітка** Ця процедура може керувати підключеннями лише в класичній програмі Outlook для Windows клієнтів. Користувач може продовжити доступ до спільних папок за допомогою OWA або Outlook для Mac.
 
Докладні відомості див. в [статтях](https://aka.ms/controlpf)Про підтримку керованих підключень до спільних папок у Outlook .