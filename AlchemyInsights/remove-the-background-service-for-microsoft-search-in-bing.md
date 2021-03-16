---
title: Видалення фонової служби для Microsoft Search у службі Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816342"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="c6dc0-102">Видалення фонової служби для Microsoft Search у службі Bing</span><span class="sxs-lookup"><span data-stu-id="c6dc0-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="c6dc0-103">Щоб видалити фонову службу для Microsoft Search у службі Bing, можна скористатися такими засобами:</span><span class="sxs-lookup"><span data-stu-id="c6dc0-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="c6dc0-104">Щоб повернутися до початкових параметрів пошукової системи, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="c6dc0-105">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-105">a.</span></span> <span data-ttu-id="c6dc0-106">Установіть перемикач **використовувати Бінг як пошукову програму за замовчуванням [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome)**.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="c6dc0-107">b.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-107">b.</span></span> <span data-ttu-id="c6dc0-108">[Перейдіть до центру адміністрування Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) і зніміть параметр, який впливає на всіх користувачів організації.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="c6dc0-109">Щоб видалити фонову службу з окремого пристрою, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="c6dc0-110">муніципалітет.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-110">a.</span></span> <span data-ttu-id="c6dc0-111">Виберіть **елемент панель керування > програми > програми та засоби**.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="c6dc0-112">b.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-112">b.</span></span> <span data-ttu-id="c6dc0-113">Клацніть правою кнопкою миші **службу Microsoft Search у службі Bing у** списку інстальованих програм, а потім натисніть кнопку **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="c6dc0-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="c6dc0-114">Щоб видалити фонову службу з кількох пристроїв у вашій організації, увійдіть у систему як адміністратор і виконайте таку команду в сценарії:</span><span class="sxs-lookup"><span data-stu-id="c6dc0-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
