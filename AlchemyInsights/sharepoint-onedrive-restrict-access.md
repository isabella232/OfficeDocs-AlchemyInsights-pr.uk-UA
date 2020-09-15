---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700476"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="4e81b-102">Обмеження доступу в SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="4e81b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="4e81b-103">Існує багато способів обмежити доступ до служб SharePoint Online або OneDrive.</span><span class="sxs-lookup"><span data-stu-id="4e81b-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="4e81b-104">Нижче наведені різні методи обмеження доступу.</span><span class="sxs-lookup"><span data-stu-id="4e81b-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="4e81b-105">**Обмеження дозволів**</span><span class="sxs-lookup"><span data-stu-id="4e81b-105">**Permission Restriction**</span></span>

<span data-ttu-id="4e81b-106">У службі SharePoint Online і "OneDrive для бізнесу" ми обмежуємо доступ до таких елементів, як сайти, файли та папки, лише надаючи доступ до цих груп або осіб, які мають доступ.</span><span class="sxs-lookup"><span data-stu-id="4e81b-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="4e81b-107">Настроювання дозволів для списку або бібліотеки SharePoint</span><span class="sxs-lookup"><span data-stu-id="4e81b-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="4e81b-108">Настроювання дозволів на сайт SharePoint</span><span class="sxs-lookup"><span data-stu-id="4e81b-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="4e81b-109">Змінення дозволів у вкладеній папці</span><span class="sxs-lookup"><span data-stu-id="4e81b-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="4e81b-110">Керування доступом із некерованих пристроїв</span><span class="sxs-lookup"><span data-stu-id="4e81b-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="4e81b-111">Як служба SharePoint або Глобальний адміністратор, ви можете блокувати або обмежувати доступ до вмісту SharePoint і OneDrive з некерованих пристроїв (ті, що не є гібридним ОГОЛОШЕННЯМ, до яких приєдналися або сумісні в Inune).</span><span class="sxs-lookup"><span data-stu-id="4e81b-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="4e81b-112">**Обмеження мережного розташування**</span><span class="sxs-lookup"><span data-stu-id="4e81b-112">**Network Location Restriction**</span></span>

<span data-ttu-id="4e81b-113">Як ІТ-адміністратор можна керувати доступом до ресурсів SharePoint і OneDrive на основі визначених мережевих розташувань, які ви довіряєте.</span><span class="sxs-lookup"><span data-stu-id="4e81b-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="4e81b-114">Цей параметр також відомий як політика на основі розташування.</span><span class="sxs-lookup"><span data-stu-id="4e81b-114">This is also known as location-based policy.</span></span> <span data-ttu-id="4e81b-115">Докладні відомості наведено в статті [керування доступом до даних SharePoint Online і OneDrive на основі мережного розташування](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location) .</span><span class="sxs-lookup"><span data-stu-id="4e81b-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="4e81b-116">**Обмеження блокування сайту**</span><span class="sxs-lookup"><span data-stu-id="4e81b-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="4e81b-117">У службі SharePoint Online ви маєте можливість заблокувати колекцію сайтів, щоб мати доступ до них.</span><span class="sxs-lookup"><span data-stu-id="4e81b-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="4e81b-118">Цей параметр настроєно через PowerShell і [оболонку керування SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) за допомогою властивості [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="4e81b-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="4e81b-119">**Обмеження користувачів зі створення сайтів і підсайтів**</span><span class="sxs-lookup"><span data-stu-id="4e81b-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="4e81b-120">Адміністратор SharePoint або Глобальний адміністратор дає змогу користувачам створювати та адмініструвати власні сайти SharePoint, визначати типи сайтів, які вони можуть створювати, а також визначати розташування сайтів.</span><span class="sxs-lookup"><span data-stu-id="4e81b-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="4e81b-121">Докладні відомості наведено [в статті керування створенням сайтів у службі SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="4e81b-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

