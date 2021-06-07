---
title: Настроювання Microsoft Intune опорних точок безпеки Windows 10 пристроями
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794126"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="36f3e-102">Настроювання Microsoft Intune опорних точок безпеки Windows 10 пристроями</span><span class="sxs-lookup"><span data-stu-id="36f3e-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="36f3e-103">Базові плани безпеки Intune допомагають захистити користувачів і пристрої.</span><span class="sxs-lookup"><span data-stu-id="36f3e-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="36f3e-104">Базові плани безпеки Windows попередньо настроєні групи, що використовуються для застосування відомої групи параметрів і значень за замовчуванням, рекомендованих відповідними командами безпеки.</span><span class="sxs-lookup"><span data-stu-id="36f3e-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="36f3e-105">Створивши профіль базового плану безпеки в Intune, ви створюєте шаблон, який складається з кількох профілів конфігурації пристрою.</span><span class="sxs-lookup"><span data-stu-id="36f3e-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="36f3e-106">Під час розгортання опорних точок безпеки для груп користувачів або пристроїв настройки застосовуються до пристроїв, які виконуються на Windows 10 або пізніших версіях.</span><span class="sxs-lookup"><span data-stu-id="36f3e-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="36f3e-107">Наприклад, базовий план керування мобільними пристроями (MDM) Microsoft автоматично вмикає BitLocker для знімних дисків, вимагає пароля для розблокування пристрою та вимкнення базової автентифікації.</span><span class="sxs-lookup"><span data-stu-id="36f3e-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="36f3e-108">Якщо стандартне значення не працює у вашому середовищі, ви можете налаштувати базовий план, щоб застосувати потрібні параметри.</span><span class="sxs-lookup"><span data-stu-id="36f3e-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="36f3e-109">Базові плани безпеки також допомагають створити найнижчий захищений робочий цикл у Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="36f3e-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="36f3e-110">Базовий план безпеки містить поради й рекомендації щодо параметрів, які впливають на безпеку.</span><span class="sxs-lookup"><span data-stu-id="36f3e-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="36f3e-111">Партнери Intune з командою Windows безпеки, яка створює базові плани для групових політик, тому ці рекомендації базуються на суцільних рекомендаціях і великому досвіді.</span><span class="sxs-lookup"><span data-stu-id="36f3e-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="36f3e-112">Якщо ви ще не знаходитесь у Intune і не знаєте, з чого почати, опорні вказівки безпеки допоможуть швидко створити й розгорнути захищений профіль.</span><span class="sxs-lookup"><span data-stu-id="36f3e-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="36f3e-113">Якщо зараз використовується групова політика, перенесення до Intune для керування значно простіше з опорними планами безпеки, оскільки вони вбудовані в Intune і включають повноцінні можливості керування.</span><span class="sxs-lookup"><span data-stu-id="36f3e-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="36f3e-114">Докладні відомості див. в [статтях Windows опорних точок безпеки та](/windows/security/threat-protection/windows-security-baselines) [Керування мобільними пристроями.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="36f3e-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

