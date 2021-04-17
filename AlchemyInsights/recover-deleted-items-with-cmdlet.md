---
title: Відновлення видалених елементів за допомогою командлета
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
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835832"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="46a75-102">Відновлення видалених елементів за допомогою командлета</span><span class="sxs-lookup"><span data-stu-id="46a75-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="46a75-103">Використовуйте командлет [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps), щоб переглядати видалені елементи в поштових скриньках.</span><span class="sxs-lookup"><span data-stu-id="46a75-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="46a75-104">Знайшовши видалені елементи, можна скористатися командлетом [Restore-RestoreableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps), щоб відновити їх.</span><span class="sxs-lookup"><span data-stu-id="46a75-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="46a75-105">Докладні відомості про командлет [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="46a75-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="46a75-106">Перш ніж запустити цей командлет, вам має бути призначено роль "Імпорт і експорт поштових скриньок".</span><span class="sxs-lookup"><span data-stu-id="46a75-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="46a75-107">Докладні відомості про командлет Get-RecoverableItems див. [тут](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="46a75-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
