---
title: Відновлення видаленого сайту
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692064"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="ffc7d-102">Відновлення видаленого сайту</span><span class="sxs-lookup"><span data-stu-id="ffc7d-102">Restore a deleted site</span></span>

<span data-ttu-id="ffc7d-103">Коли адміністратор видаляє сайт SharePoint, його буде розміщено в кошику колекції сайтів, де він зберігається протягом 93 днів, перш ніж його остаточно видалено.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="ffc7d-104">Щоб відновити сайт, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-104">To restore the site:</span></span>
  
1. <span data-ttu-id="ffc7d-105">У новому центрі адміністрування SharePoint натисніть кнопку **кошик** на стрічці.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="ffc7d-106">Установіть прапорець поруч із колекцією сайтів, яку потрібно відновити.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="ffc7d-107">Натисніть кнопку **відновити видалені елементи**.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="ffc7d-108">Щоб відновити видалений сайт спілкування, можна скористатися новим центром адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="ffc7d-109">В іншому разі потрібно використовувати Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="ffc7d-110">Щоб відновити сайт, який належить до групи Microsoft 365, потрібно відновити групу в центрі адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="ffc7d-111">Групи можна відновити протягом 30 днів після видалення.</span><span class="sxs-lookup"><span data-stu-id="ffc7d-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

