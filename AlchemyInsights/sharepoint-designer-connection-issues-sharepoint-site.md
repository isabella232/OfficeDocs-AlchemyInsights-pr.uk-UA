---
title: Проблеми з підключенням до конструктора SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511565"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="34200-102">Проблеми з підключенням до конструктора SharePoint</span><span class="sxs-lookup"><span data-stu-id="34200-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="34200-103">Якщо SharePoint Designer переживає проблеми з підключенням до сайтів SharePoint, спробуйте скористатися такими загальними рішеннями.</span><span class="sxs-lookup"><span data-stu-id="34200-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="34200-104">Крок 1: переконайтеся, що SharePoint Designer 2013 оновлено [SharePoint Designer з пакетом оновлень 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) і [2 серпня 2016 оновлення для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="34200-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="34200-105">Крок 2: очистіть локальні файли кешу:</span><span class="sxs-lookup"><span data-stu-id="34200-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="34200-106">Закрийте SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="34200-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="34200-107">На локальному комп'ютері видаліть усі файли, знайдені в кожній з таких папок.</span><span class="sxs-lookup"><span data-stu-id="34200-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="34200-108">%Appind%\mempice\веб-сервер розширення \ кеш</span><span class="sxs-lookup"><span data-stu-id="34200-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="34200-109">%Appind%\mempice\sharepoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="34200-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="34200-110">% Userпрофільні%\appind\locm</span><span class="sxs-lookup"><span data-stu-id="34200-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="34200-111">Відкрийте SharePoint Designer 2013 і знову введіть обліковий запис, щоб побачити, чи працює він.</span><span class="sxs-lookup"><span data-stu-id="34200-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="34200-112">Крок 3: [Увімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="34200-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="34200-113">Крок 4: адміністраторам потрібно **дозволити користувацький скрипт** у настройках центру адміністрування SharePoint, щоб дозволити підключення конструктора SharePoint.</span><span class="sxs-lookup"><span data-stu-id="34200-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="34200-114">Щоб отримати додаткові відомості [,](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) див.</span><span class="sxs-lookup"><span data-stu-id="34200-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


