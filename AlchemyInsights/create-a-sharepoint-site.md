---
title: Створення сайту SharePoint
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36738218"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="1a2ff-102">Створення сайту SharePoint</span><span class="sxs-lookup"><span data-stu-id="1a2ff-102">Create a SharePoint site</span></span>

<span data-ttu-id="1a2ff-103">Для отримання відомостей про створення сайту SharePoint можна переглянути такі відомості:</span><span class="sxs-lookup"><span data-stu-id="1a2ff-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="1a2ff-104">[Керування сайтами в новому центрі адміністрування SharePoint](https://docs.microsoft.com/sharepoint/manage-site-creation): Дізнайтеся про параметри створення сайту, зокрема, як створити класичний сайт або сайт teams, який не містить групи Office 365.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="1a2ff-105">[Створіть сайт групи в SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Дізнайтеся, як створити сайт групи.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="1a2ff-106">[Створення сайту зв'язку в SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Дізнайтеся, як створити сайт зв'язку.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="1a2ff-107">[Керування сайтами в новому центрі адміністрування SharePoint](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Дізнайтеся, як створити класичний сайт або сайт групи, який не містить групи Office 365.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="1a2ff-108">[! Поради</span><span class="sxs-lookup"><span data-stu-id="1a2ff-108">[!Tips]</span></span>
> - <span data-ttu-id="1a2ff-109">Не можна створити сайт з однаковою URL-адресою наявного сайту.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="1a2ff-110">Якщо ви видалили сайт і бажаєте повторно використовувати URL, можливо, видалений сайт все ще існує в розділі **Видалені сайти**.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="1a2ff-111">Щоб керувати видаленими сайтами, [видаліть сайт](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="1a2ff-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="1a2ff-112">Щоб повністю видалити сайт за допомогою PowerShell, див. [](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="1a2ff-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="1a2ff-113">Деякі користувачі не зможуть створити сайт.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="1a2ff-114">Дивіться [керування створенням сайту в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="1a2ff-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="1a2ff-115">Можливо, на сайті з'являється застрягли при **створенні** довше, ніж очікувалося.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="1a2ff-116">Якщо Минуло більше 24 годин з тих пір, як ви вперше побачили цю проблему, будь ласка, увійдіть квиток підтримки.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="1a2ff-117">У багатьох випадках ми вже працюємо над вирішенням.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="1a2ff-118">Будь ласка, дайте нам принаймні 24 годин, щоб завершити рішення.</span><span class="sxs-lookup"><span data-stu-id="1a2ff-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="1a2ff-119">Якщо потрібно створити новий сайт групи, який не містить групи Office 365,</span><span class="sxs-lookup"><span data-stu-id="1a2ff-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


