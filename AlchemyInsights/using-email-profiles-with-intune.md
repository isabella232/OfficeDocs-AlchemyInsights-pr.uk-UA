---
title: Використання профілів електронної пошти з InTune
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
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555757"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="89deb-102">Використання профілів електронної пошти з InTune</span><span class="sxs-lookup"><span data-stu-id="89deb-102">Using email profiles with Intune</span></span>

<span data-ttu-id="89deb-103">InTune можна використовувати для створення та розгортання профілів електронної пошти для власного (вбудованого) поштового клієнта на кількох платформах пристрою.</span><span class="sxs-lookup"><span data-stu-id="89deb-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="89deb-104">Для отримання відомостей про деякі обмеження, пов'язані з профілями електронної пошти, зокрема про те, як обробляються наявні профілі та як видаляти профілі [електронної пошти, див.](https://docs.microsoft.com/intune/email-settings-configure)</span><span class="sxs-lookup"><span data-stu-id="89deb-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="89deb-105">Щоб отримати додаткові відомості про створення профілів електронної пошти для кожної платформи пристрою, див.:</span><span class="sxs-lookup"><span data-stu-id="89deb-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="89deb-106">Налаштування пристрою Android для налаштування електронної пошти, аутентифікації та синхронізації в InTune</span><span class="sxs-lookup"><span data-stu-id="89deb-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="89deb-107">Додавання параметрів електронної пошти для пристроїв iOS і Ipадос у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="89deb-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="89deb-108">Параметри профілю електронної пошти в Microsoft InTune для пристроїв під керуванням Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="89deb-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="89deb-109">Параметри профілю електронної пошти для пристроїв під керуванням Windows 10 у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="89deb-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="89deb-110">**Поширені проблеми синхронізації**</span><span class="sxs-lookup"><span data-stu-id="89deb-110">**Common syncing issue**</span></span>

<span data-ttu-id="89deb-111">**НОКС на Android профіль електронної пошти забороняє користувачам контакти, календар і завдання, від синхронізації до користувача пристроїв.**</span><span class="sxs-lookup"><span data-stu-id="89deb-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="89deb-112">НОКС на андроїд НОКС профіль електронної пошти пропонує адміністратору можливість вирішити, які типи вмісту синхронізуються з пристроєм, встановивши кожен включений.</span><span class="sxs-lookup"><span data-stu-id="89deb-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="89deb-113">Якщо параметр для будь-якого типу вмісту налаштовано **не настроєно** (за промовчанням), цей тип вмісту не синхронізуватиметься автоматично.</span><span class="sxs-lookup"><span data-stu-id="89deb-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="89deb-114">Користувач може ввімкнути тип вмісту, який вони хочуть безпосередньо на пристрої вручну, але цю конфігурацію буде перезаписано параметром політики InTune, а для цього типу вмісту припиняється синхронізація.</span><span class="sxs-lookup"><span data-stu-id="89deb-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

