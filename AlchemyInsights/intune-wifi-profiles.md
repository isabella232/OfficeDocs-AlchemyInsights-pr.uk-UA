---
title: InTune профілі Wi-Fi
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555818"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="e6f84-102">InTune профілі Wi-Fi</span><span class="sxs-lookup"><span data-stu-id="e6f84-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="e6f84-103">Успішне впровадження Wi-Fi підключення для клієнтів MDM залежить від правильно розгорнутого профілю, який відображає вимоги корпоративної інфраструктури Wi-Fi.</span><span class="sxs-lookup"><span data-stu-id="e6f84-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="e6f84-104">Щоб переглянути відповідні параметри для клієнтських платформ, які ви розслідували, див.:</span><span class="sxs-lookup"><span data-stu-id="e6f84-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="e6f84-105">Додавання настройок Wi-Fi для пристроїв під керуванням ОС Android у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="e6f84-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="e6f84-106">Додавання параметрів Wi-Fi для Android Enterprise, присвячених і повністю керованих пристроїв у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="e6f84-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="e6f84-107">Додавання параметрів Wi-Fi для пристроїв iOS і Ipадос у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="e6f84-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="e6f84-108">Додавання настройок Wi-Fi для Windows 10 і пізніших пристроїв у InTune</span><span class="sxs-lookup"><span data-stu-id="e6f84-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="e6f84-109">Імпорт параметрів Wi-Fi для пристроїв Windows у InTune</span><span class="sxs-lookup"><span data-stu-id="e6f84-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="e6f84-110">**Поширених проблем**</span><span class="sxs-lookup"><span data-stu-id="e6f84-110">**Common Issues**</span></span>

<span data-ttu-id="e6f84-111">**Я розгорнула профіль Wi-Fi, що залежить від розгорнутого сертифіката, вказаного в профілі Wi-Fi. Однак, профілі конфігурації відображаються стан помилки.**</span><span class="sxs-lookup"><span data-stu-id="e6f84-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="e6f84-112">Переконайтеся, що ваш пристрій отримав сертифікат.</span><span class="sxs-lookup"><span data-stu-id="e6f84-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="e6f84-113">У InTune перейдіть до **всіх пристроїв** і виберіть пристрій > **конфігурацію пристрою**.</span><span class="sxs-lookup"><span data-stu-id="e6f84-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="e6f84-114">Переконайтеся, що всі очікувані профілі перелічені та в успішному стані.</span><span class="sxs-lookup"><span data-stu-id="e6f84-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="e6f84-115">Для профілю Android, якщо у ланцюжку сертифікатів є проміжні сертифікати, переконайтеся, що вони розгорнуті на пристроях Android.</span><span class="sxs-lookup"><span data-stu-id="e6f84-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="e6f84-116">Щоб перевірити стан сертифіката, перейдіть до **пристрою**  >  **профілі**конфігурації  >  **Android проміжні**  >  **Властивості**CA  >  **довірений сертифікат**.</span><span class="sxs-lookup"><span data-stu-id="e6f84-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="e6f84-117">Якщо ви продовжуєте бачити помилки, перегляньте розділи процедури та виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="e6f84-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="e6f84-118">Щоб отримати додаткові відомості див [Огляд для виправлення неполадок SCEP, профілі сертифікатів, з Microsoft InTune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e6f84-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="e6f84-119">**Я розгорнула профіль Wi-Fi на пристрій. InTune показує, що він був успішним, але пристрій не підключається до Wi-Fi.**</span><span class="sxs-lookup"><span data-stu-id="e6f84-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="e6f84-120">Успішний стан означає, що InTune успішно розгорнуто конфігурацію, як настроєно.</span><span class="sxs-lookup"><span data-stu-id="e6f84-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="e6f84-121">Проте ці конфігурації можуть не відповідати вимогам для мережі та/або автентифікації.</span><span class="sxs-lookup"><span data-stu-id="e6f84-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="e6f84-122">Щоб отримати докладніші відомості про спробу підключення, перегляньте журнали в службі інфраструктури та автентифікації (на контролері точки доступу Wi-Fi і сервері NPS/радіус).</span><span class="sxs-lookup"><span data-stu-id="e6f84-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="e6f84-123">Можливо, доведеться працювати з командою мережної інфраструктури або постачальником Wi-Fi сторонніх виробників, щоб збирати й рецензувати журнали.</span><span class="sxs-lookup"><span data-stu-id="e6f84-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>