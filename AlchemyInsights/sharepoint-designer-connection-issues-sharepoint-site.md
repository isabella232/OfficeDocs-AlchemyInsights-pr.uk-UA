---
title: SharePoint Designer і FTP-клієнти
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508444"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="0f8bf-102">SharePoint Designer і FTP-клієнти</span><span class="sxs-lookup"><span data-stu-id="0f8bf-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="0f8bf-103">Якщо SharePoint Designer переживає питання, підключення до сайтів SharePoint, будь ласка, спробуйте такі спільні рішення.</span><span class="sxs-lookup"><span data-stu-id="0f8bf-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="0f8bf-104">Крок 1: Переконайтеся, що SharePoint Designer 2013 оновлюється з [пакета оновлень 1 для SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) і [2 серпня 2016 оновлення для SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="0f8bf-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="0f8bf-105">Крок 2: Очистити кеш локальних файлів:</span><span class="sxs-lookup"><span data-stu-id="0f8bf-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="0f8bf-106">Закрийте SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="0f8bf-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="0f8bf-107">На локальному комп'ютері видалити всі файли у кожному із таких папок.</span><span class="sxs-lookup"><span data-stu-id="0f8bf-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="0f8bf-108">%AppData%\Microsoft\Web сервер Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="0f8bf-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="0f8bf-109">%AppData%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="0f8bf-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="0f8bf-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="0f8bf-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="0f8bf-111">Відкрити SharePoint Designer 2013 і введіть обліковий запис знову, щоб побачити, якщо вона працює.</span><span class="sxs-lookup"><span data-stu-id="0f8bf-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="0f8bf-112">Крок 3: [ввімкнення сучасних автентифікації для Office 2013 на пристроях Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="0f8bf-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="0f8bf-113">Крок 4: Адміністратори повинні **Дозволити користувацький скрипт** в настройках центру адміністрування SharePoint дозволити підключення застосунку SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="0f8bf-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="0f8bf-114">Див [дозволити або заборонити власний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) для отримання додаткової інформації.</span><span class="sxs-lookup"><span data-stu-id="0f8bf-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


