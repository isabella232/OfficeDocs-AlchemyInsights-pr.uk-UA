---
title: Використання профілів електронної пошти за допомогою функції Inune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653309"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="d520c-102">Використання профілів електронної пошти за допомогою функції Inune</span><span class="sxs-lookup"><span data-stu-id="d520c-102">Using email profiles with Intune</span></span>

<span data-ttu-id="d520c-103">Inune можна використовувати для створення та розгортання профілів електронної пошти для рідного (вбудованого) поштового клієнта на пристроях з кількома пристроями.</span><span class="sxs-lookup"><span data-stu-id="d520c-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="d520c-104">Щоб отримати відомості про деякі обмеження, пов'язані з профілями електронної пошти, зокрема про те, як обробляється наявність наявного профілю, і як видалити профілі електронної пошти, перегляньте статтю [Додавання настройок електронної пошти до пристроїв із використанням функції Inune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="d520c-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="d520c-105">Щоб отримати докладні відомості про те, як створювати профілі електронної пошти для кожної платформи пристроїв, ознайомтеся з такими можливостями:</span><span class="sxs-lookup"><span data-stu-id="d520c-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="d520c-106">Параметри пристрою з Android для настроювання електронної пошти, автентифікації та синхронізації в програмі Inune</span><span class="sxs-lookup"><span data-stu-id="d520c-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="d520c-107">Додавання настройок електронної пошти для пристроїв iOS і iPadOS в Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="d520c-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="d520c-108">Параметри профілю електронної пошти в Microsoft Inteune для пристроїв під керуванням ОС Windows Phone 8,1</span><span class="sxs-lookup"><span data-stu-id="d520c-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="d520c-109">Параметри профілю електронної пошти для пристроїв під керуванням ОС Windows 10 у Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="d520c-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="d520c-110">**Звичайна помилка синхронізації**</span><span class="sxs-lookup"><span data-stu-id="d520c-110">**Common syncing issue**</span></span>

<span data-ttu-id="d520c-111">**У "НОКС" в профілі електронної пошти Android запобігає синхронізації контактів користувачів, календаря та завдань, а не синхронізувати їх із пристроями користувача.**</span><span class="sxs-lookup"><span data-stu-id="d520c-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="d520c-112">У профілі "НОКС" на пристрої з Android KNOX, у якому наведено адміністратор, можна визначити типи вмісту, які потрібно синхронізувати з пристроєм, встановивши кожен із них.</span><span class="sxs-lookup"><span data-stu-id="d520c-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="d520c-113">Якщо параметр для будь-якого типу вмісту налаштовано **не настроєно** (за замовчуванням), цей тип вмісту не синхронізується автоматично.</span><span class="sxs-lookup"><span data-stu-id="d520c-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="d520c-114">Користувач може ввімкнути тип вмісту, який потрібно безпосередньо на пристрої вручну, але ця конфігурація замінюється параметром політики Inune, а синхронізація зупиняється для цього типу вмісту.</span><span class="sxs-lookup"><span data-stu-id="d520c-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

