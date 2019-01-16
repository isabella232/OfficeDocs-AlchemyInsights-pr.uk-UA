---
title: Активувати аудит поштової скриньки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: bd94ec10f9df2e72ec6e3d8552d2eb80212a9d78
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318687"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="544a0-102">Активувати аудит поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="544a0-102">Enable mailbox auditing</span></span>

<span data-ttu-id="544a0-103">Щоб активувати аудит поштової скриньки для одного користувача або всією установою наведені нижче команди cmdlet має бути запущено з віддаленої оболонки живлення:</span><span class="sxs-lookup"><span data-stu-id="544a0-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="544a0-104">**Одного користувача**</span><span class="sxs-lookup"><span data-stu-id="544a0-104">**Single User**</span></span>
  
<span data-ttu-id="544a0-105">Set-Mailbox - ідентичності "Джейн Доу" - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="544a0-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="544a0-106">**Organization**</span><span class="sxs-lookup"><span data-stu-id="544a0-106">**Organization**</span></span>
  
<span data-ttu-id="544a0-107">Get-Mailbox - ResultSize необмежений - фільтрувати {"UserMailbox", RecipientTypeDetails - eq} | Set-Mailbox - AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="544a0-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="544a0-108">Додаткові відомості</span><span class="sxs-lookup"><span data-stu-id="544a0-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

