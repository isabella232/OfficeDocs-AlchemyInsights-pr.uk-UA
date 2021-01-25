---
title: Поштову скриньку архіву майже заповнено
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974668"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="a9164-102">Поштову скриньку архіву майже заповнено</span><span class="sxs-lookup"><span data-stu-id="a9164-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="a9164-103">Якщо користувач отримує попередження; **Поштова скринька архіву майже повна** або потрібно збільшити розмір поштової скриньки архіву, ось кілька порад:</span><span class="sxs-lookup"><span data-stu-id="a9164-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="a9164-104">Якщо для користувача призначено план Exchange Online 1, оновіть ліцензію на службу **Exchange Online Plan 2** , щоб збільшити розмір від 50 ГБ до 100 ГБ.</span><span class="sxs-lookup"><span data-stu-id="a9164-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="a9164-105">Якщо користувач уже призначається один із таких пунктів: **Exchange Online Plan 2** або Exchange Online Plan 1 із надбудовою архівування Exchange Online, виконайте наведені нижче дії, щоб активувати автоматичне розширення архівації:.</span><span class="sxs-lookup"><span data-stu-id="a9164-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="a9164-106">[Підключіться до Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="a9164-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="a9164-107">Виконайте такі дії чином для користувача:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="a9164-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="a9164-108">Виконайте наведені нижче чином, щоб підтвердити, що його активовано для користувача.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="a9164-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="a9164-109">Докладні відомості наведено в статті:</span><span class="sxs-lookup"><span data-stu-id="a9164-109">For more information see:</span></span>

- [<span data-ttu-id="a9164-110"> Активувати необмежену архівацію – Довідка для адміністратора – відповідність вимогам Microsoft 365 | Документи Microsoft</span><span class="sxs-lookup"><span data-stu-id="a9164-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="a9164-111">Обмеження Exchange Online – описи служб | Документи Microsoft</span><span class="sxs-lookup"><span data-stu-id="a9164-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="a9164-112">Оновлення до іншої бізнес-плану | Документи Microsoft</span><span class="sxs-lookup"><span data-stu-id="a9164-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

