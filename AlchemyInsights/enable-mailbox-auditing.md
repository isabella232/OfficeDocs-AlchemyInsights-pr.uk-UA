---
title: Увімкнути аудит поштової скриньки
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736274"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="e4152-102">Увімкнути аудит поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="e4152-102">Enable mailbox auditing</span></span>

<span data-ttu-id="e4152-103">Щоб увімкнути аудит поштової скриньки для одного користувача або всієї організації, потрібно запустити такі командлети з віддаленої оболонки живлення:</span><span class="sxs-lookup"><span data-stu-id="e4152-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="e4152-104">**Одного користувача**</span><span class="sxs-lookup"><span data-stu-id="e4152-104">**Single User**</span></span>
  
<span data-ttu-id="e4152-105">Set-поштова скринька-Identity "Джейн Доу"-аудита $true</span><span class="sxs-lookup"><span data-stu-id="e4152-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="e4152-106">**Організації**</span><span class="sxs-lookup"><span data-stu-id="e4152-106">**Organization**</span></span>
  
<span data-ttu-id="e4152-107">Get-поштова скринька-розмір необмежений фільтр {RecipientTypeDetails-EQ "UserMailbox скринька"} | Набір-поштова скринька-можливість аудита $true</span><span class="sxs-lookup"><span data-stu-id="e4152-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="e4152-108">Дізнатися більше</span><span class="sxs-lookup"><span data-stu-id="e4152-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

