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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="d8a0c-102">Увімкнення DKIM для певного домену за допомогою служби Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="d8a0c-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="d8a0c-103">Якщо не вдалося створити записи DNS DKIM в центрі адміністрування, скористайтеся засобом Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d8a0c-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="d8a0c-104">Щоб створити запис DNS DKIM за допомогою служби Exchange Online PowerShell, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="d8a0c-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="d8a0c-105">Відкрийте Windows PowerShell як адміністратор і виконайте наведені нижче команди в описаній послідовності.</span><span class="sxs-lookup"><span data-stu-id="d8a0c-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="d8a0c-106">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="d8a0c-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="d8a0c-107">b.</span><span class="sxs-lookup"><span data-stu-id="d8a0c-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="d8a0c-108">c.</span><span class="sxs-lookup"><span data-stu-id="d8a0c-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="d8a0c-109">Якщо у вас виникли проблеми з підключенням до Exchange Online PowerShell, перегляньте статтю [підключитися до Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="d8a0c-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="d8a0c-110">Коли ви підключаєтеся до Exchange Online PowerShell, виконайте таку команду:</span><span class="sxs-lookup"><span data-stu-id="d8a0c-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="d8a0c-111">Після успішного виконання команди, виконайте таку команду, щоб завершити сеанс Exchange Online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d8a0c-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



