---
title: Увімкнення DKIM для певного домену за допомогою служби Exchange Online PowerShell
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749735"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Увімкнення DKIM для певного домену за допомогою служби Exchange Online PowerShell

Якщо не вдалося створити записи DNS DKIM в центрі адміністрування, скористайтеся засобом Exchange Online PowerShell. 

Щоб створити запис DNS DKIM за допомогою служби Exchange Online PowerShell, виконайте наведені нижче дії.

1. Відкрийте Windows PowerShell як адміністратор і виконайте наведені нижче команди в описаній послідовності.

    муніципалітет. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Якщо у вас виникли проблеми з підключенням до Exchange Online PowerShell, перегляньте статтю [підключитися до Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Коли ви підключаєтеся до Exchange Online PowerShell, виконайте таку команду:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Після успішного виконання команди, виконайте таку команду, щоб завершити сеанс Exchange Online PowerShell:

    `Remove-PSSession $Session` 



