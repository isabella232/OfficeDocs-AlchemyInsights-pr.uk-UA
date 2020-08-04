---
title: Проблеми, пов'язані з VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555741"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="5e814-102">Проблеми, пов'язані з VPN</span><span class="sxs-lookup"><span data-stu-id="5e814-102">VPN related issues</span></span>

<span data-ttu-id="5e814-103">Успішне виконання VPN-підключення для клієнтів MDM залежить від розгорнутого профілю, який правильно відображає вимоги інфраструктури VPN.</span><span class="sxs-lookup"><span data-stu-id="5e814-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="5e814-104">Для відповідних параметрів для клієнтських платформ, які ви розслідували, див.:</span><span class="sxs-lookup"><span data-stu-id="5e814-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="5e814-105">Windows 10 і параметри голографічного пристрою Windows для додавання підключень VPN за допомогою InTune</span><span class="sxs-lookup"><span data-stu-id="5e814-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="5e814-106">Додайте настройки VPN на пристроях iOS і Ipадос у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="5e814-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="5e814-107">Налаштування пристрою Android для налаштування VPN у InTune</span><span class="sxs-lookup"><span data-stu-id="5e814-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="5e814-108">Додавання настройок VPN на пристроях macOS у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="5e814-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="5e814-109">Якщо ваш профіль VPN використовує автентифікацію на основі сертифіката, переконайтеся, що кореневі сертифікати та профілі сертифікатів автентифікації клієнта, зв'язані з профілем VPN, успішно розгорнуті.</span><span class="sxs-lookup"><span data-stu-id="5e814-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="5e814-110">**Поширених проблем**</span><span class="sxs-lookup"><span data-stu-id="5e814-110">**Common Issues**</span></span>

<span data-ttu-id="5e814-111">**Я розгорнула профіль VPN на пристрій. InTune показує, що це було успішно, але пристрій не підключається до мережі VPN.**</span><span class="sxs-lookup"><span data-stu-id="5e814-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="5e814-112">Успішний стан означає, що InTune успішно розгорнуто конфігурацію, як настроєно.</span><span class="sxs-lookup"><span data-stu-id="5e814-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="5e814-113">Проте ці конфігурації можуть не відповідати вимогам для мережі та/або автентифікації.</span><span class="sxs-lookup"><span data-stu-id="5e814-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="5e814-114">Перегляньте журнали в службі інфраструктури та автентифікації (на сервері VPN і NPS/радіус сервера) для отримання додаткових відомостей про спробу підключення.</span><span class="sxs-lookup"><span data-stu-id="5e814-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="5e814-115">Можливо, потрібно буде працювати з командою мережної інфраструктури або постачальником VPN сторонніх постачальників, щоб збирати журнали та переглядати їх.</span><span class="sxs-lookup"><span data-stu-id="5e814-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="5e814-116">**Коли я налаштовую VPN для iOS, функція для VPN для додатків недоступна.**</span><span class="sxs-lookup"><span data-stu-id="5e814-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="5e814-117">На додаток VPN для iOS пристроїв у InTune в даний час доступна для певного списку постачальників і партнерів, які також повинні відповідати на сертифікати передумови перед настроюванням на додаток VPN.</span><span class="sxs-lookup"><span data-stu-id="5e814-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="5e814-118">Для отримання додаткових відомостей див. [налаштування віртуальної приватної мережі (VPN) для пристроїв IOS/Ipадос у InTune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span><span class="sxs-lookup"><span data-stu-id="5e814-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="5e814-119">Щоб отримати додаткові відомості про всі типи підключення VPN у InTune, див. [створення ПРОФІЛІВ VPN для підключення до СЕРВЕРІВ VPN у InTune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="5e814-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="5e814-120">**iOS на вимогу VPN не запуск під час доступу до настроєного домену**</span><span class="sxs-lookup"><span data-stu-id="5e814-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="5e814-121">Щоб перевірити автоматичні настройки VPN, установіть такі значення:</span><span class="sxs-lookup"><span data-stu-id="5e814-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="5e814-122">Я хочу зробити наступне: **оцінити кожну спробу підключення**</span><span class="sxs-lookup"><span data-stu-id="5e814-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="5e814-123">Виберіть, чи слід підключатися: **підключатися, якщо потрібно**</span><span class="sxs-lookup"><span data-stu-id="5e814-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="5e814-124">Коли користувачі мають доступ до цих доменів: **цільове** *доменне ім'я*</span><span class="sxs-lookup"><span data-stu-id="5e814-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="5e814-125">Якщо вищезазначена конфігурація не успішна, додайте наступний елемент:</span><span class="sxs-lookup"><span data-stu-id="5e814-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="5e814-126">Якщо ця URL-адреса недоступна, примусово підключіть VPN: **Badurl**</span><span class="sxs-lookup"><span data-stu-id="5e814-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>