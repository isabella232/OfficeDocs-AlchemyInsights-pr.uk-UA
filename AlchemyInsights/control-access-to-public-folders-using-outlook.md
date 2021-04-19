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
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816761"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Керування доступом до спільних папок за допомогою Outlook

Щоб визначити, які користувачі мають доступ до спільних папок, за допомогою Outlook:

1. Використання `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: надання користувачам доступу до спільних папок в Outlook  
$false. Заборона доступу користувачів до спільних папок в Outlook. ; ; ;Це значення за замовчуванням.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Примітка. Ця процедура може керувати підключеннями лише з класичною програмою Outlook для windows. Користувачі можуть і надалі отримувати доступ до спільних папок за допомогою OWA або Outlook для Mac.

Докладні відомості див. в статтях Керовані підключення до спільних папок [у програмі Outlook.](https://aka.ms/controlpf)
