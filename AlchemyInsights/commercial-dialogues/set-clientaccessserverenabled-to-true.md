---
title: Настроювання значення "для сервера"
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749972"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="0e678-102">Настроювання значення "для сервера"</span><span class="sxs-lookup"><span data-stu-id="0e678-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="0e678-103">Якщо ви не можете відкрити зашифроване повідомлення електронної пошти, а натомість побачити вкладення **rрmsg** , виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="0e678-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="0e678-104">Підключіться до Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0e678-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="0e678-105">Щоб підключитися до служби Exchange Online PowerShell, потрібно ввійти за допомогою глобального адміністратора або облікового запису Exchange адміністратора.</span><span class="sxs-lookup"><span data-stu-id="0e678-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="0e678-106">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="0e678-106">a.</span></span> <span data-ttu-id="0e678-107">Відкрийте Windows PowerShell, а потім виконайте таку команду: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="0e678-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="0e678-108">b.</span><span class="sxs-lookup"><span data-stu-id="0e678-108">b.</span></span> <span data-ttu-id="0e678-109">У діалоговому вікні **запит облікових даних Windows PowerShell** введіть свій робоча або навчальний обліковий запис і пароль, c.</span><span class="sxs-lookup"><span data-stu-id="0e678-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="0e678-110">Натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="0e678-110">Click **OK**.</span></span> 

2. <span data-ttu-id="0e678-111">Щоб створити новий сеанс, виконайте таку команду:</span><span class="sxs-lookup"><span data-stu-id="0e678-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="0e678-112">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="0e678-112">a.</span></span> <span data-ttu-id="0e678-113">Запустіть таку команду:</span><span class="sxs-lookup"><span data-stu-id="0e678-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="0e678-114">Команда «виконати `Get-IRMConfiguration` ».</span><span class="sxs-lookup"><span data-stu-id="0e678-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="0e678-115">Установіть прапорець поруч із параметром **Clienacc"** .</span><span class="sxs-lookup"><span data-stu-id="0e678-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="0e678-116">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="0e678-116">a.</span></span> <span data-ttu-id="0e678-117">Якщо параметр **Clienacceserverenувімкнуто** , установлено значення **false**, запустіть наведений нижче командлет. `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="0e678-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="0e678-118">Завжди закривайте сеанс PowerShell за допомогою наведеної нижче команди. `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="0e678-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="0e678-119">Докладні відомості наведено в статті [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="0e678-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

