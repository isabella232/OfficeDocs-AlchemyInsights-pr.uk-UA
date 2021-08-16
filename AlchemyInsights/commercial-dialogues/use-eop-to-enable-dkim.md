---
title: Увімкнення Exchange Online DKIM для певного домену за допомогою PowerShell
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070345"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Увімкнення Exchange Online DKIM для певного домену за допомогою PowerShell

Якщо не вдається створити записи DNS DKIM у Центрі адміністрування, спробуйте скористатися Exchange Online PowerShell. 

Щоб створити запис DNS DKIM за допомогою Exchange Online PowerShell, виконайте такі дії:

1. Відкрийте Windows PowerShell як адміністратор і виконайте наведені нижче команди в описаних послідовності.

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Якщо у вас виникли проблеми з підключенням Exchange Online PowerShell, [див. Підключення до Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Підключившися до Exchange Online PowerShell, виконайте таку команду:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Після успішного виконання наведеної вище команди виконайте таку команду, щоб припинити сеанс Exchange Online PowerShell:

    `Remove-PSSession $Session` 



