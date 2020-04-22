---
title: Увімкнути аудит поштової скриньки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: ae11d6be0789a5662d202b85268480a3d42922c4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703592"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="ef945-102">Увімкнути аудит поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="ef945-102">Enable mailbox auditing</span></span>

<span data-ttu-id="ef945-103">Щоб увімкнути аудит поштової скриньки для одного користувача або всієї організації, потрібно запустити такі командлети з віддаленої оболонки живлення:</span><span class="sxs-lookup"><span data-stu-id="ef945-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="ef945-104">**Одного користувача**</span><span class="sxs-lookup"><span data-stu-id="ef945-104">**Single User**</span></span>
  
<span data-ttu-id="ef945-105">Set-поштова скринька-Identity "Джейн Доу"-аудита $true</span><span class="sxs-lookup"><span data-stu-id="ef945-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="ef945-106">**Організації**</span><span class="sxs-lookup"><span data-stu-id="ef945-106">**Organization**</span></span>
  
<span data-ttu-id="ef945-107">Get-поштова скринька-розмір необмежений фільтр {RecipientTypeDetails-EQ "UserMailbox скринька"} | Набір-поштова скринька-можливість аудита $true</span><span class="sxs-lookup"><span data-stu-id="ef945-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="ef945-108">Дізнатися більше</span><span class="sxs-lookup"><span data-stu-id="ef945-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

