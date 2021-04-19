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
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="edd90-102">Керування доступом до спільних папок за допомогою Outlook</span><span class="sxs-lookup"><span data-stu-id="edd90-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="edd90-103">Щоб визначити, які користувачі мають доступ до спільних папок, за допомогою Outlook:</span><span class="sxs-lookup"><span data-stu-id="edd90-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="edd90-104">Використання `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="edd90-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="edd90-105">$true: надання користувачам доступу до спільних папок в Outlook</span><span class="sxs-lookup"><span data-stu-id="edd90-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="edd90-106">$false. Заборона доступу користувачів до спільних папок в Outlook.</span><span class="sxs-lookup"><span data-stu-id="edd90-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="edd90-107">; ; ;Це значення за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="edd90-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="edd90-108">Примітка. Ця процедура може керувати підключеннями лише з класичною програмою Outlook для windows.</span><span class="sxs-lookup"><span data-stu-id="edd90-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="edd90-109">Користувачі можуть і надалі отримувати доступ до спільних папок за допомогою OWA або Outlook для Mac.</span><span class="sxs-lookup"><span data-stu-id="edd90-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="edd90-110">Докладні відомості див. в статтях Керовані підключення до спільних папок [у програмі Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="edd90-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
