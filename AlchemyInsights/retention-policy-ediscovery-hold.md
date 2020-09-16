---
title: 2609 – збереження або відкриття – утримання
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727912"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="3675d-102">Не вдається видалити елементи в службі SharePoint Online або OneDrive для бізнесу</span><span class="sxs-lookup"><span data-stu-id="3675d-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="3675d-103">Ви або ваші користувачі не зможуть видаляти елементи в службі SharePoint Online або OneDrive для бізнесу, тому що політика збереження, підпис збереження або утримання eDiscovery застосовуються до SharePoint сайту OneDrive або до певного елемента.</span><span class="sxs-lookup"><span data-stu-id="3675d-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="3675d-104">Це включає в себе не вдалося видалити документ, версію документа, папку, бібліотеку документів, список, програму, сайт або колекцію сайтів.</span><span class="sxs-lookup"><span data-stu-id="3675d-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="3675d-105">Щоб видалити елементи в одному з цих сценаріїв, потрібно видалити політику збереження, мітку збереження або утримання електронної інформації (або сайт має бути виключено з політики збереження).</span><span class="sxs-lookup"><span data-stu-id="3675d-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="3675d-106">Потрібно вимкнути або виключити відповідне утримання, що спричиняє цю проблему.</span><span class="sxs-lookup"><span data-stu-id="3675d-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="3675d-107">Після видалення політики збереження або утримання може знадобитися до 24 годин, щоб зміни набрали сили.</span><span class="sxs-lookup"><span data-stu-id="3675d-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="3675d-108">Щоб отримати відомості про різні функції збереження та утримання, які можна застосувати до сайтів SharePoint і облікових записів OneDrive, ознайомтеся з однією з наведених нижче розділів.</span><span class="sxs-lookup"><span data-stu-id="3675d-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="3675d-109">Загальні відомості про політики збереження</span><span class="sxs-lookup"><span data-stu-id="3675d-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="3675d-110">Огляд міток збереження</span><span class="sxs-lookup"><span data-stu-id="3675d-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="3675d-111">Керування утриманнями в розширеному Витребування електронної інформації</span><span class="sxs-lookup"><span data-stu-id="3675d-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="3675d-112">Пошук у Витребування електронної інформації</span><span class="sxs-lookup"><span data-stu-id="3675d-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="3675d-113">Застарілі політики закриття та видалення сайтів</span><span class="sxs-lookup"><span data-stu-id="3675d-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)