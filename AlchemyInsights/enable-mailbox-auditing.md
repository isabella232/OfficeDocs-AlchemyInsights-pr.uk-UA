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
ms.openlocfilehash: 2bcfb7cc174cd58b21e1bb0c82f0d7cdb25e2fdd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506975"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="8083c-102">Увімкнути аудит поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="8083c-102">Enable mailbox auditing</span></span>

<span data-ttu-id="8083c-103">Щоб увімкнути аудит поштової скриньки для одного користувача або всієї організації, потрібно запустити такі командлети з віддаленої оболонки живлення:</span><span class="sxs-lookup"><span data-stu-id="8083c-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="8083c-104">**Одного користувача**</span><span class="sxs-lookup"><span data-stu-id="8083c-104">**Single User**</span></span>
  
<span data-ttu-id="8083c-105">Set-поштова скринька-Identity "Джейн Доу"-аудита $true</span><span class="sxs-lookup"><span data-stu-id="8083c-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="8083c-106">**Організації**</span><span class="sxs-lookup"><span data-stu-id="8083c-106">**Organization**</span></span>
  
<span data-ttu-id="8083c-107">Get-поштова скринька-розмір необмежений фільтр {RecipientTypeDetails-EQ "UserMailbox скринька"} | Набір-поштова скринька-можливість аудита $true</span><span class="sxs-lookup"><span data-stu-id="8083c-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="8083c-108">Дізнатися більше</span><span class="sxs-lookup"><span data-stu-id="8083c-108">Learn more</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-mailbox-auditing)
  

