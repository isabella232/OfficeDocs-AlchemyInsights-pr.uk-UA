---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692786"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="97769-102">Обмеження доступу в SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="97769-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="97769-103">Існує багато способів обмежити доступ до служб SharePoint Online/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="97769-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="97769-104">Ці різні методи обмеження доступу викладені нижче.</span><span class="sxs-lookup"><span data-stu-id="97769-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="97769-105">**Обмеження доступу**</span><span class="sxs-lookup"><span data-stu-id="97769-105">**Permission Restriction**</span></span>

<span data-ttu-id="97769-106">У SharePoint Online та OneDrive для бізнесу ми обмежуємо доступ до таких елементів, як сайти, файли та папки, лише надаючи доступ до цих груп/осіб, які мають доступ.</span><span class="sxs-lookup"><span data-stu-id="97769-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="97769-107">Настроювання дозволів для списку або бібліотеки SharePoint</span><span class="sxs-lookup"><span data-stu-id="97769-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="97769-108">Настроювання дозволів сайту SharePoint</span><span class="sxs-lookup"><span data-stu-id="97769-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="97769-109">Змінення дозволів у вкладеній папці</span><span class="sxs-lookup"><span data-stu-id="97769-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="97769-110">Керування доступом із некерованих пристроїв</span><span class="sxs-lookup"><span data-stu-id="97769-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="97769-111">Як SharePoint або Глобальний адміністратор ви можете заблокувати або обмежити доступ до вмісту SharePoint і OneDrive з некерованих пристроїв (це не гібридні оголошення, які приєдналися або сумісні в InTune).</span><span class="sxs-lookup"><span data-stu-id="97769-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="97769-112">**Обмеження розташування мережі**</span><span class="sxs-lookup"><span data-stu-id="97769-112">**Network Location Restriction**</span></span>

<span data-ttu-id="97769-113">Як ІТ-адміністратор ви можете керувати доступом до ресурсів SharePoint і OneDrive на основі визначених мережевих розташувань, яким ви довіряєте.</span><span class="sxs-lookup"><span data-stu-id="97769-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="97769-114">Це також відоме як політика на основі розташування.</span><span class="sxs-lookup"><span data-stu-id="97769-114">This is also known as location-based policy.</span></span> <span data-ttu-id="97769-115">Для отримання додаткових відомостей зверніться до [керування доступом до SharePoint Online та OneDrive даних на основі мережного розташування](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="97769-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="97769-116">**Обмеження блокування сайту**</span><span class="sxs-lookup"><span data-stu-id="97769-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="97769-117">У SharePoint Online у вас є можливість заблокувати колекцію сайтів, тому ніхто не має доступу.</span><span class="sxs-lookup"><span data-stu-id="97769-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="97769-118">Це встановлено за допомогою PowerShell і [оболонки керування SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , використовуючи властивість [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -локстан.</span><span class="sxs-lookup"><span data-stu-id="97769-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="97769-119">**Як заборонити користувачам створювати сайти або підсайти**</span><span class="sxs-lookup"><span data-stu-id="97769-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="97769-120">Як адміністратор SharePoint або Глобальний адміністратор ви можете дозволити користувачам створювати та адмініструвати власні сайти SharePoint, визначати, які сайти вони можуть створювати, і вказувати розташування сайтів.</span><span class="sxs-lookup"><span data-stu-id="97769-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="97769-121">Для отримання додаткової інформації, будь ласка, дивіться [керування створенням сайту в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="97769-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

