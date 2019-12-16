---
title: Як відновити видалений сайт
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: edf851da951e163f30660d524049abe0798a8314
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048817"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="18700-102">Як відновити видалений сайт</span><span class="sxs-lookup"><span data-stu-id="18700-102">Restore a deleted site</span></span>

<span data-ttu-id="18700-103">Коли адміністратор видаляє сайт SharePoint, він поміщається в кошик колекції сайтів, де він зберігається протягом 93 днів, перш ніж його остаточно видалити.</span><span class="sxs-lookup"><span data-stu-id="18700-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="18700-104">Щоб відновити сайт:</span><span class="sxs-lookup"><span data-stu-id="18700-104">To restore the site:</span></span>
  
1. <span data-ttu-id="18700-105">У новому центрі адміністрування SharePoint клацніть піктограму **кошик** на стрічці.</span><span class="sxs-lookup"><span data-stu-id="18700-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="18700-106">Установіть прапорці поруч із колекцією сайтів, які потрібно відновити.</span><span class="sxs-lookup"><span data-stu-id="18700-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="18700-107">Натисніть кнопку **відновити видалені елементи**.</span><span class="sxs-lookup"><span data-stu-id="18700-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="18700-108">Щоб відновити видалений сайт зв'язку, можна використовувати новий Центр адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="18700-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="18700-109">В іншому випадку потрібно використовувати Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="18700-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="18700-110">Щоб відновити сайт, який належить до групи Office 365, потрібно відновити групу в центрі адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="18700-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="18700-111">Групи можна відновити протягом 30 днів після їх видалення.</span><span class="sxs-lookup"><span data-stu-id="18700-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

