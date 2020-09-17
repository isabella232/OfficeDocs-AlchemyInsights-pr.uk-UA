---
title: Створення сайту SharePoint
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806960"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="301b9-102">Створення сайту SharePoint</span><span class="sxs-lookup"><span data-stu-id="301b9-102">Create a SharePoint site</span></span>

<span data-ttu-id="301b9-103">Створюйте сайти та керуйте ними на сайтах із [активних сайтів](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) у центрі адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="301b9-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="301b9-104">Докладні відомості наведено в статті [керування сайтами в новому центрі адміністрування SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="301b9-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="301b9-105">Поради</span><span class="sxs-lookup"><span data-stu-id="301b9-105">Tips:</span></span>

- <span data-ttu-id="301b9-106">**Не** можна створити сайт з тією самою URL-адресою наявного сайту.</span><span class="sxs-lookup"><span data-stu-id="301b9-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="301b9-107">Якщо ви видалили сайт і хочете повторно використовувати URL-адресу, можливо, видалений сайт все ще перебуває в розділі [Видалені сайти](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="301b9-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="301b9-108">Щоб повторно використовувати URL-адресу, сайт знадобиться остаточно видалити.</span><span class="sxs-lookup"><span data-stu-id="301b9-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="301b9-109">Щоб повністю видалити сайт із PowerShell, перегляньте приклад командлета [Видалити-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) .</span><span class="sxs-lookup"><span data-stu-id="301b9-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="301b9-110">Можливо, деякі користувачі не зможуть створити сайт.</span><span class="sxs-lookup"><span data-stu-id="301b9-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="301b9-111">[Перегляньте статтю керування створенням сайту в службі SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="301b9-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="301b9-112">Можливо, сайт застряг на час **створення** довше, ніж очікувалося.</span><span class="sxs-lookup"><span data-stu-id="301b9-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="301b9-113">Якщо ви вперше побачили цю проблему понад 24 години, увійдіть у службу підтримки.</span><span class="sxs-lookup"><span data-stu-id="301b9-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="301b9-114">У багатьох випадках ми вже працюємо над вирішенням проблеми.</span><span class="sxs-lookup"><span data-stu-id="301b9-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="301b9-115">Щоб завершити вирішення, надайте нам принаймні 24 години.</span><span class="sxs-lookup"><span data-stu-id="301b9-115">Please give us at least 24 hours to complete a solution.</span></span>
