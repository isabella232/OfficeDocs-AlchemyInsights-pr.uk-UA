---
title: Керування веб-доступом у Microsoft Edge для iOS і Android за допомогою Microsoft Intune
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989728"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="1b94a-102">Керування веб-доступом у Microsoft Edge для iOS і Android за допомогою Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1b94a-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="1b94a-103">Microsoft Edge для iOS і Android дає користувачу змогу переглядати веб-сторінки з кількох окремих профілів.</span><span class="sxs-lookup"><span data-stu-id="1b94a-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="1b94a-104">Найширші можливості захисту даних Microsoft 365 стають доступними, коли ви передплатили пакет Enterprise Mobility + Security, до якого входять Microsoft Intune і Azure Active Directory Premium, як-от умовний доступ.</span><span class="sxs-lookup"><span data-stu-id="1b94a-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="1b94a-105">Принаймні потрібно розгорнути політику умовного доступу, яка (1) дає змогу користувачам підключатися з мобільних пристроїв до Microsoft Edge для iOS і Android і що (2) впроваджує політику захисту програм Microsoft Intune, яка забезпечує захищений перегляд веб-сторінок.</span><span class="sxs-lookup"><span data-stu-id="1b94a-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="1b94a-106">Щоб зрозуміти, як можна використовувати умовний доступ і політики, див. статті:</span><span class="sxs-lookup"><span data-stu-id="1b94a-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="1b94a-107">Застосування політик умовного доступу Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1b94a-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="1b94a-108">Створення політик захисту програм Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1b94a-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="1b94a-109">Використання єдиного входу для веб-програм, підключених до Azure Active Directory, у браузерах, захищених політикою</span><span class="sxs-lookup"><span data-stu-id="1b94a-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="1b94a-110">Використовуйте конфігурацію програми для керування переглядом</span><span class="sxs-lookup"><span data-stu-id="1b94a-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="1b94a-111">Дозволити використання лише робочих і навчальних облікових записів</span><span class="sxs-lookup"><span data-stu-id="1b94a-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="1b94a-112">Розгортання загальних політик конфігурації програм</span><span class="sxs-lookup"><span data-stu-id="1b94a-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="1b94a-113">Розгортання політик конфігурації програм для захисту даних</span><span class="sxs-lookup"><span data-stu-id="1b94a-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="1b94a-114">Розгортання політик конфігурації програми за допомогою Microsoft Endpoint Manager</span><span class="sxs-lookup"><span data-stu-id="1b94a-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="1b94a-115">Відомості про те, як отримати доступ до журналів керованих програм, див. в статті Доступ до журналів керованих програм за допомогою Microsoft Edge для [iOS і Android.](https://go.microsoft.com/fwlink/?linkid=2132578)</span><span class="sxs-lookup"><span data-stu-id="1b94a-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
