---
title: Не вдається отримати доступ до спільних папок
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812568"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="13227-102">Outlook не вдається підключитися до спільних папок</span><span class="sxs-lookup"><span data-stu-id="13227-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="13227-103">Якщо доступ до спільної папки не працює для деяких користувачів, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="13227-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="13227-104">Підключіться до EXO PowerShell і настройте параметр "Def" за промовчанням у обліковому записі користувача, щоб відповідати параметру для робочого облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="13227-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="13227-105">Наприклад</span><span class="sxs-lookup"><span data-stu-id="13227-105">Example:</span></span>

<span data-ttu-id="13227-106">Початок роботи з поштовою скринькою | FT Def"поштова скринька", "ефективність" для поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="13227-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="13227-107">Настроювання – поштова скринька для неавтоматичного користувача – за промовчанням \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="13227-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="13227-108">Зачекайте принаймні одну годину, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="13227-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="13227-109">Якщо проблему не вирішено, виконайте [цю процедуру](https://aka.ms/pfcte) , щоб виправити неполадки з доступом до спільної папки за допомогою програми Outlook.</span><span class="sxs-lookup"><span data-stu-id="13227-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="13227-110">**Щоб керувати доступом користувачів до спільних папок за допомогою програми Outlook**, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="13227-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="13227-111">Використання Set-CASMailbox <mailboxname> – публікаклієнтський доступ $TRUE або $FALSE</span><span class="sxs-lookup"><span data-stu-id="13227-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="13227-112">$true: дозволити користувачам отримувати доступ до спільних папок у програмі Outlook</span><span class="sxs-lookup"><span data-stu-id="13227-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="13227-113">$false: заборонити доступ користувачів до спільних папок у програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="13227-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="13227-114">; ; ;Це значення за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="13227-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="13227-115">Настроювання – OrganizationConfig – публікаціями $true</span><span class="sxs-lookup"><span data-stu-id="13227-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="13227-116">**Примітка** . У цій процедурі можна керувати підключеннями лише з робочим столом Outlook для клієнтів Windows.</span><span class="sxs-lookup"><span data-stu-id="13227-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="13227-117">Користувач може продовжити доступ до спільних папок за допомогою OWA або Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="13227-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="13227-118">Докладні відомості наведено в статті [оголошення про підтримку керованих підключень до спільних папок у програмі Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="13227-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>