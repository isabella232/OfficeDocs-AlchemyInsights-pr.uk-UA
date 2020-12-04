---
title: Настроювання пристроїв із Windows 10 за допомогою базових планів безпеки Microsoft Inune
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573784"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="ece12-102">Настроювання пристроїв із Windows 10 за допомогою базових планів безпеки Microsoft Inune</span><span class="sxs-lookup"><span data-stu-id="ece12-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="ece12-103">Під час використання базових планів безпеки захист користувачів і пристроїв.</span><span class="sxs-lookup"><span data-stu-id="ece12-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ece12-104">Базові параметри безпеки – це попередньо настроєні групи параметрів Windows, які використовуються для застосування відомої групи параметрів і значень за замовчуванням, рекомендованих відповідними групами безпеки.</span><span class="sxs-lookup"><span data-stu-id="ece12-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ece12-105">Створюючи базовий профіль безпеки в програмі Inune, ви створюєте шаблон, що складається з кількох профілів конфігурації пристрою.</span><span class="sxs-lookup"><span data-stu-id="ece12-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ece12-106">Під час розгортання базових планів безпеки для груп користувачів або пристроїв ці параметри застосовуються до пристроїв, які виконуються в ОС Windows 10 або новіших версіях.</span><span class="sxs-lookup"><span data-stu-id="ece12-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="ece12-107">Наприклад, за допомогою програми BitLocker для знімних дисків (1) можна автоматично використовувати базовий план безпеки, що дає змогу використовувати пароль для розблокування пристрою, і (3) відключає базову автентифікацію.</span><span class="sxs-lookup"><span data-stu-id="ece12-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ece12-108">Якщо значення за замовчуванням не працює для вашого середовища, настройте базову лінію, щоб використовувати потрібні параметри.</span><span class="sxs-lookup"><span data-stu-id="ece12-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ece12-109">Базові параметри безпеки також сприяють встановленню безпечного робочого циклу в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ece12-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ece12-110">Нижче наведено деякі переваги цього:</span><span class="sxs-lookup"><span data-stu-id="ece12-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="ece12-111">Базова лінія безпеки включає поради та рекомендації щодо параметрів, які впливають на безпеку.</span><span class="sxs-lookup"><span data-stu-id="ece12-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ece12-112">Оскільки програма Inune співпрацює з командою безпеки Windows, яка створює базові умови для групових політик, ці рекомендації базуються на ретельному керівництві та обширному досвіді.</span><span class="sxs-lookup"><span data-stu-id="ece12-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ece12-113">Якщо ви не знаєте, де можна почати роботу, а також не впевнені, що потрібно зробити, а базові параметри безпеки допоможуть швидко створити та розгорнути захищений профіль.</span><span class="sxs-lookup"><span data-stu-id="ece12-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ece12-114">Якщо ви зараз використовуєте групову політику, а потім перехід до веб-програми для керування, набагато простіше за допомогою базових планів безпеки, тому що вони вбудовані у веб-програму та включають в себе передові можливості для керування.</span><span class="sxs-lookup"><span data-stu-id="ece12-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ece12-115">Щоб дізнатися більше, ознайомтеся з [базовими лініями безпеки](https://go.microsoft.com/fwlink/?linkid=2141503) та [керування мобільними пристроями](https://go.microsoft.com/fwlink/?linkid=2141701)в ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="ece12-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>