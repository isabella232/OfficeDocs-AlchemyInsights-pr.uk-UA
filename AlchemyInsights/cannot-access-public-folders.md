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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="bec43-102">Outlook не може підключитися до спільних папок</span><span class="sxs-lookup"><span data-stu-id="bec43-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="bec43-103">Якщо доступ до спільної папки не працює для деяких користувачів, спробуйте зробити ось що:</span><span class="sxs-lookup"><span data-stu-id="bec43-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="bec43-104">Підключіться до EXO PowerShell і настройте параметр DefaultPublicFolderMailbox в обліковому записі користувача, який відповідає параметру робочого облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="bec43-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="bec43-105">Приклад.</span><span class="sxs-lookup"><span data-stu-id="bec43-105">Example:</span></span>

<span data-ttu-id="bec43-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="bec43-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="bec43-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="bec43-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="bec43-108">Зачекайте принаймні годину, доки зміни наберуть сили.</span><span class="sxs-lookup"><span data-stu-id="bec43-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="bec43-109">Якщо проблема не зсунеться, виконайте [цю процедуру,](https://aka.ms/pfcte) щоб усунути проблеми доступу до спільної папки за допомогою Outlook.</span><span class="sxs-lookup"><span data-stu-id="bec43-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="bec43-110">**Щоб визначити, які користувачі мають доступ до спільних папок, за допомогою Outlook, див.**</span><span class="sxs-lookup"><span data-stu-id="bec43-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="bec43-111">Використання Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true або $false</span><span class="sxs-lookup"><span data-stu-id="bec43-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="bec43-112">$true: надання користувачам доступу до спільних папок в Outlook</span><span class="sxs-lookup"><span data-stu-id="bec43-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="bec43-113">$false. Заборона доступу користувачів до спільних папок в Outlook.</span><span class="sxs-lookup"><span data-stu-id="bec43-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="bec43-114">; ; ;Це значення за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="bec43-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="bec43-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="bec43-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="bec43-116">**Примітка** Ця процедура може керувати підключеннями лише з класичною програмою Outlook для клієнтів Windows.</span><span class="sxs-lookup"><span data-stu-id="bec43-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="bec43-117">Користувач може і надалі отримувати доступ до спільних папок за допомогою OWA або Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="bec43-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="bec43-118">Докладні відомості див. в статтях Про підтримку керованих підключень до [спільних папок в Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="bec43-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>