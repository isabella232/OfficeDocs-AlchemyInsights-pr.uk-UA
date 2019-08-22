---
title: Обмеження доступу в SharePoint або OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559898"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="6f228-102">Обмеження доступу в SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="6f228-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="6f228-103">Є багато способів для обмеження доступу до служб SharePoint на сайті/OneDrive.</span><span class="sxs-lookup"><span data-stu-id="6f228-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="6f228-104">Ці різні методи обмеження доступу викладені нижче.</span><span class="sxs-lookup"><span data-stu-id="6f228-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="6f228-105">**Обмеження дозволів**</span><span class="sxs-lookup"><span data-stu-id="6f228-105">**Permission Restriction**</span></span>

<span data-ttu-id="6f228-106">У SharePoint Online і OneDrive для бізнесу ми заборонити доступ до пунктам, як сайти, файли та папки, тільки надання доступу до цих груп/особи, які повинні мати доступ.</span><span class="sxs-lookup"><span data-stu-id="6f228-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="6f228-107">Настроювання дозволів для списку або бібліотеки</span><span class="sxs-lookup"><span data-stu-id="6f228-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="6f228-108">Настроїти дозволи сайту SharePoint</span><span class="sxs-lookup"><span data-stu-id="6f228-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="6f228-109">Змінити дозволи на вкладену папку</span><span class="sxs-lookup"><span data-stu-id="6f228-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="6f228-110">Керування доступом від некерованих пристроїв</span><span class="sxs-lookup"><span data-stu-id="6f228-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="6f228-111">SharePoint або глобального адміністратора, у службі Office 365, ви можете блокувати або обмежити доступ до SharePoint і OneDrive вміст від некерованих пристроїв (ті не гібридних оголошення об'єднуваних або сумісний в Intune).</span><span class="sxs-lookup"><span data-stu-id="6f228-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="6f228-112">**Обмеження розташування мережі**</span><span class="sxs-lookup"><span data-stu-id="6f228-112">**Network Location Restriction**</span></span>

<span data-ttu-id="6f228-113">Як адміністратор можна контролювати доступ до SharePoint і OneDrive ресурсів на основі визначених мережних розташуваннях, яким ви довіряєте.</span><span class="sxs-lookup"><span data-stu-id="6f228-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="6f228-114">Це також відомо як місцезнаходженням політики.</span><span class="sxs-lookup"><span data-stu-id="6f228-114">This is also known as location-based policy.</span></span> <span data-ttu-id="6f228-115">Для отримання додаткової інформації будь ласка, дивіться [керування доступом до SharePoint Online і OneDrive даних на основі мережне розташування](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="6f228-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="6f228-116">**Сайт блокування обмеження**</span><span class="sxs-lookup"><span data-stu-id="6f228-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="6f228-117">У SharePoint на сайті у вас є можливість блокування колекції сайтів, так що ніхто не має доступу.</span><span class="sxs-lookup"><span data-stu-id="6f228-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="6f228-118">Це встановити за допомогою PowerShell і [SharePoint онлайн оболонки керування](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) властивістю - LockState [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="6f228-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="6f228-119">**Заборонити користувачам створення сайтів чи дочірні сайти**</span><span class="sxs-lookup"><span data-stu-id="6f228-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="6f228-120">Як адміністратор SharePoint або Office 365 глобального адміністратора, можна дозволити користувачам створювати і управляти свої власні сайти SharePoint, визначити, якого роду сайти вони можуть створити і вкажіть розташування сайтів.</span><span class="sxs-lookup"><span data-stu-id="6f228-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="6f228-121">Для отримання додаткової інформації будь ласка, дивіться [Створення сайту керування в SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="6f228-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

