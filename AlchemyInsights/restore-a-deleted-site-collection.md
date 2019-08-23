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
ms.openlocfilehash: 9e4e9ade058c60ecd7a6ce1b2a40c4996ac5676f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36552503"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="3d765-102">Відновлення видаленої сайту</span><span class="sxs-lookup"><span data-stu-id="3d765-102">Restore a deleted site</span></span>

<span data-ttu-id="3d765-103">Коли адміністратор видаляє сайт, його поміщають в колекції сайтів кошика, де вона зберігається на 93 днів, перш ніж вона видаляється остаточно.</span><span class="sxs-lookup"><span data-stu-id="3d765-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="3d765-104">Щоб відновити сайт:</span><span class="sxs-lookup"><span data-stu-id="3d765-104">To restore the site:</span></span>
  
1. <span data-ttu-id="3d765-105">Нові центру адміністрування SharePoint клацніть **«Кошик»** на стрічці.</span><span class="sxs-lookup"><span data-stu-id="3d765-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="3d765-106">Установіть прапорець поруч із колекції сайтів, для відновлення.</span><span class="sxs-lookup"><span data-stu-id="3d765-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="3d765-107">Натисніть кнопку **відновити видалені елементи**.</span><span class="sxs-lookup"><span data-stu-id="3d765-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="3d765-108">Щоб відновити видалене повідомлення сайту, можна використовувати нові центру адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="3d765-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="3d765-109">В іншому випадку ви повинні використовувати Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3d765-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="3d765-110">Щоб відновити сайт, що належить до групи Office 365, потрібно буде відновити група Exchange центру адміністрування.</span><span class="sxs-lookup"><span data-stu-id="3d765-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="3d765-111">Групи можуть бути відновлені протягом 30 днів після того, як вони ви видалили.</span><span class="sxs-lookup"><span data-stu-id="3d765-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

