---
title: Відновлення видаленої сайту
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 0cf10a3a0effc1774d8a07c5d0be96384362c175
ms.sourcegitcommit: 228c986911ecf73217116a5d1fdcd2e89362774e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/09/2019
ms.locfileid: "31747799"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="14393-102">Відновлення видаленої сайту</span><span class="sxs-lookup"><span data-stu-id="14393-102">Restore a deleted site</span></span>

<span data-ttu-id="14393-103">Коли адміністратор видаляє сайт, його поміщають в колекції сайтів кошика, де вона зберігається на 93 днів, перш ніж вона видаляється остаточно.</span><span class="sxs-lookup"><span data-stu-id="14393-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="14393-104">Щоб відновити сайт:</span><span class="sxs-lookup"><span data-stu-id="14393-104">To restore the site:</span></span>
  
1. <span data-ttu-id="14393-105">Нові центру адміністрування SharePoint клацніть **«Кошик»** на стрічці.</span><span class="sxs-lookup"><span data-stu-id="14393-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="14393-106">Установіть прапорець поруч із колекції сайтів, для відновлення.</span><span class="sxs-lookup"><span data-stu-id="14393-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="14393-107">Натисніть кнопку **відновити видалені елементи**.</span><span class="sxs-lookup"><span data-stu-id="14393-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="14393-108">Щоб відновити видалене повідомлення сайту, можна використовувати нові центру адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="14393-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="14393-109">В іншому випадку ви повинні використовувати Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="14393-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="14393-110">Щоб відновити сайт, що належить до групи Office 365, потрібно буде відновити група Exchange центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="14393-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="14393-111">Групи можуть бути відновлені протягом 30 днів після того, як вони ви видалили.</span><span class="sxs-lookup"><span data-stu-id="14393-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

