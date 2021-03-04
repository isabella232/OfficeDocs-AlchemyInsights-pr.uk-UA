---
title: Увімкнення аудиту поштової скриньки
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430247"
---
# <a name="turn-on-mailbox-auditing"></a><span data-ttu-id="71e4e-102">Увімкнення аудиту поштової скриньки</span><span class="sxs-lookup"><span data-stu-id="71e4e-102">Turn on mailbox auditing</span></span>

<span data-ttu-id="71e4e-103">Щоб увімкнути аудит поштової скриньки для одного користувача або всієї організації, запустіть наведені нижче командлети з віддаленого PowerShell:</span><span class="sxs-lookup"><span data-stu-id="71e4e-103">To turn on mailbox auditing for a single user or an entire organization, run the following cmdlets from Remote PowerShell:</span></span>

- <span data-ttu-id="71e4e-104">**Єдиний користувач**: Set-Mailbox-ідентичність "Джейн Dow" – AuditEnabled $True</span><span class="sxs-lookup"><span data-stu-id="71e4e-104">**Single user**: Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
- <span data-ttu-id="71e4e-105">**Організація**: Get-Mailbox-ResultSize Unlimited-Filter {Reseientype(дані)-еквалайзер "usermailbox"} | Set-Mailbox-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="71e4e-105">**Organization**: Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>

<span data-ttu-id="71e4e-106">Докладні відомості наведено в статті [керування аудиторською поштовою скринькою](https://go.microsoft.com/fwlink/?linkid=2103668).</span><span class="sxs-lookup"><span data-stu-id="71e4e-106">To learn more, see [Manage mailbox auditing](https://go.microsoft.com/fwlink/?linkid=2103668).</span></span>