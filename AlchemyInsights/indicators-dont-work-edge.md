---
title: Індикатори не працюють у браузері Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676575"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="4ffcd-102">Індикатори не працюють у браузері Edge</span><span class="sxs-lookup"><span data-stu-id="4ffcd-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="4ffcd-103">Якщо ви створили індикатор, його не вражено в Edge (фільтр Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="4ffcd-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="4ffcd-104">Докладні відомості див. [в розділі Створення індикаторів для IPs, URL-адрес або доменів.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="4ffcd-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="4ffcd-105">Крок 1. Переконайтеся, що:</span><span class="sxs-lookup"><span data-stu-id="4ffcd-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="4ffcd-106">Переконайтеся, що індикатор правильний (неправильно введено IP-адресу або URL-адресу, правильні дії, правильні групи RBAC).</span><span class="sxs-lookup"><span data-stu-id="4ffcd-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="4ffcd-107">Зачекайте 2 години після створення індикатора, щоб врахувати будь-яку можливу затримку.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="4ffcd-108">Переконайтеся, що систему до'єднано до Microsoft Defender для кінцевої точки.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="4ffcd-109">Переконайтеся, що системи можуть спілкуватися з хмарою.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="4ffcd-110">Переконайтеся, що фільтр Smartscreen увімкнуто й доступний, перейшовте на [тестовий сайт.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="4ffcd-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="4ffcd-111">Крок 2. Усунення потенційної проблеми</span><span class="sxs-lookup"><span data-stu-id="4ffcd-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="4ffcd-112">Переконайтеся, що клієнт відповідає вимогам.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="4ffcd-113">Докладні відомості [див. в розділі Створення індикаторів для IPs, URL-адрес або доменів.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="4ffcd-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="4ffcd-114">Переконайтеся, що ви використовуєте найновішу версію браузера Edge.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="4ffcd-115">Відомості про те, як дізнатися останню версію, див. в [Microsoft Edge.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="4ffcd-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="4ffcd-116">Перезапустіть браузер Edge.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="4ffcd-117">Перейдіть на сайт, для якого налаштоться індикатор.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="4ffcd-118">Якщо сайт відображається ненадійно, перейдіть до кроку 3.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="4ffcd-119">Крок 3. Збирання даних</span><span class="sxs-lookup"><span data-stu-id="4ffcd-119">Step 3: Collect data</span></span>

- <span data-ttu-id="4ffcd-120">Збирати **діагностичні дані MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="4ffcd-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="4ffcd-121">Інструкції див. в [статті Проблеми з приєднуванням до Microsoft Defender для кінцевої точки.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="4ffcd-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="4ffcd-122">Якщо ви вмієте інсталювати й збирати трасування Fiddler, див. дія програми [Telerik Fiddler.](http://www.telerik.com/fiddler)</span><span class="sxs-lookup"><span data-stu-id="4ffcd-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="4ffcd-123">Якщо ви віддаєте перевагу інструкціям від служби підтримки Microsoft, клацніть піктограму підтримки нижче, щоб відкрити інцидент служби підтримки.</span><span class="sxs-lookup"><span data-stu-id="4ffcd-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
