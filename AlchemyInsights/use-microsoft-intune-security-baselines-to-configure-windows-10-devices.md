---
title: Використання базових планів безпеки Microsoft Inune для настроювання пристроїв із Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696386"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="e5db5-102">Використання базових планів безпеки Microsoft Inune для налаштування пристроїв із Windows 10</span><span class="sxs-lookup"><span data-stu-id="e5db5-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="e5db5-103">Під час використання базових планів безпеки захист користувачів і пристроїв.</span><span class="sxs-lookup"><span data-stu-id="e5db5-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="e5db5-104">Базові параметри безпеки – це попередньо настроєні групи параметрів Windows, які використовуються для застосування відомої групи параметрів і значень за замовчуванням, рекомендованих відповідними групами безпеки.</span><span class="sxs-lookup"><span data-stu-id="e5db5-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="e5db5-105">Створюючи базовий профіль безпеки в програмі Inune, ви створюєте шаблон, що складається з кількох профілів конфігурації пристрою.</span><span class="sxs-lookup"><span data-stu-id="e5db5-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="e5db5-106">Під час розгортання базових планів безпеки для груп користувачів або пристроїв ці параметри застосовуються до пристроїв, які виконуються в ОС Windows 10 або новіших версіях.</span><span class="sxs-lookup"><span data-stu-id="e5db5-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="e5db5-107">Наприклад, автоматично базова лінія безпеки для мобільних пристроїв Microsoft (1) дає змогу програмі BitLocker для знімних дисків (2) використовувати пароль для розблокування пристрою, а (3) вимикає базову автентифікацію.</span><span class="sxs-lookup"><span data-stu-id="e5db5-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="e5db5-108">Якщо значення за замовчуванням не працює для вашого середовища, можна настроїти базову лінію, щоб використовувати потрібні параметри.</span><span class="sxs-lookup"><span data-stu-id="e5db5-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="e5db5-109">Базові параметри безпеки також сприяють встановленню безпечного робочого циклу в Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="e5db5-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="e5db5-110">Нижче наведено деякі переваги цієї функції.</span><span class="sxs-lookup"><span data-stu-id="e5db5-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="e5db5-111">Базова лінія безпеки включає поради та рекомендації щодо параметрів, які впливають на безпеку.</span><span class="sxs-lookup"><span data-stu-id="e5db5-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="e5db5-112">Оскільки програма Inune співпрацює з командою безпеки Windows, яка створює базові умови для групових політик, ці рекомендації базуються на ретельному керівництві та обширному досвіді.</span><span class="sxs-lookup"><span data-stu-id="e5db5-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="e5db5-113">Якщо ви не знаєте, де можна почати роботу, а також не впевнені, що потрібно зробити, а базові параметри безпеки допоможуть швидко створити та розгорнути захищений профіль.</span><span class="sxs-lookup"><span data-stu-id="e5db5-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="e5db5-114">Якщо ви зараз використовуєте групову політику, а потім перенесення до Inune для цілей керування набагато простіше з базовими лініями безпеки, оскільки ці опорні точки безпеки вбудовано в програму, а також мають можливість використовувати передові можливості для керування.</span><span class="sxs-lookup"><span data-stu-id="e5db5-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="e5db5-115">Докладні відомості наведено в статті [опорні точки безпеки Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) і [керування мобільними пристроями](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="e5db5-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>