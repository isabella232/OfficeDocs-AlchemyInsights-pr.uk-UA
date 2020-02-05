---
title: Створення сайту SharePoint
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770876"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="abf3e-102">Створення сайту SharePoint</span><span class="sxs-lookup"><span data-stu-id="abf3e-102">Create a SharePoint site</span></span>

<span data-ttu-id="abf3e-103">Створення сайтів або керування ними з [активних сайтів](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) у центрі адміністрування SharePoint.</span><span class="sxs-lookup"><span data-stu-id="abf3e-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="abf3e-104">Для отримання додаткових відомостей див. [керування сайтами в новому центрі адміністрування SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="abf3e-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="abf3e-105">Поради:</span><span class="sxs-lookup"><span data-stu-id="abf3e-105">Tips:</span></span>

- <span data-ttu-id="abf3e-106">**Не можна** створити сайт з однаковою URL-адресою наявного сайту.</span><span class="sxs-lookup"><span data-stu-id="abf3e-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="abf3e-107">Якщо ви видалили сайт і бажаєте повторно використовувати URL, можливо, видалений сайт все ще існує в розділі [Видалені сайти](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="abf3e-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="abf3e-108">Сайт потрібно буде остаточно видалити, щоб повторно використовувати URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="abf3e-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="abf3e-109">Щоб повністю видалити сайт за допомогою PowerShell, див. [](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="abf3e-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="abf3e-110">Деякі користувачі не зможуть створити сайт.</span><span class="sxs-lookup"><span data-stu-id="abf3e-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="abf3e-111">[Дивіться керування створенням сайту в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="abf3e-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="abf3e-112">Можливо, на сайті з'являється застрягли при **створенні** довше, ніж очікувалося.</span><span class="sxs-lookup"><span data-stu-id="abf3e-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="abf3e-113">Якщо Минуло більше 24 годин з тих пір, як ви вперше побачили цю проблему, будь ласка, увійдіть квиток підтримки.</span><span class="sxs-lookup"><span data-stu-id="abf3e-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="abf3e-114">У багатьох випадках ми вже працюємо над вирішенням.</span><span class="sxs-lookup"><span data-stu-id="abf3e-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="abf3e-115">Будь ласка, дайте нам принаймні 24 годин, щоб завершити рішення.</span><span class="sxs-lookup"><span data-stu-id="abf3e-115">Please give us at least 24 hours to complete a solution.</span></span>
