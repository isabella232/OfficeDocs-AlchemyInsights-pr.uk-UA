---
title: Диспетчер кінцевих точок – базові плани безпеки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421217"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="7b40f-102">Диспетчер кінцевих точок – базові плани безпеки</span><span class="sxs-lookup"><span data-stu-id="7b40f-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="7b40f-103">Опорні плани безпеки – це попередньо настроєні групи параметрів Windows, які допомагають застосовувати параметри безпеки, рекомендовані відповідними командами безпеки.</span><span class="sxs-lookup"><span data-stu-id="7b40f-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="7b40f-104">Ці базові плани можна налаштувати так, щоб вони надали лише потрібні параметри та значення.</span><span class="sxs-lookup"><span data-stu-id="7b40f-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="7b40f-105">Докладні відомості про базові плани безпеки див. в статті Налаштування пристроїв Windows 10 в Intune за допомогою [базових планів безпеки.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="7b40f-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="7b40f-106">Зараз для цих продуктів є такі опорні плани:</span><span class="sxs-lookup"><span data-stu-id="7b40f-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="7b40f-107">Настройки безпеки Windows MDM</span><span class="sxs-lookup"><span data-stu-id="7b40f-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="7b40f-108">Microsoft Defender для безпеки кінцевих точок</span><span class="sxs-lookup"><span data-stu-id="7b40f-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="7b40f-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="7b40f-109">Microsoft Edge</span></span>

<span data-ttu-id="7b40f-110">Оновлення кожного з базових планів періодично та випускатимуться інкрементними версіями.</span><span class="sxs-lookup"><span data-stu-id="7b40f-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="7b40f-111">Кожна версія додає або видаляє параметри з попередньої версії, щоб переконатися, що базовий план відповідає поточним вказівкам.</span><span class="sxs-lookup"><span data-stu-id="7b40f-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="7b40f-112">Консоль опорних точок безпеки в модулі endpoint Security дає змогу порівнювати різні версії, вносячи зміни з версії на видиму.</span><span class="sxs-lookup"><span data-stu-id="7b40f-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="7b40f-113">Докладні відомості про те, як найефективніше змінити версію базового плану, див. в статті Керування профілями базового плану безпеки [в Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="7b40f-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="7b40f-114">Розгорнувши базовий план безпеки, можна відстежувати стан розгортання та перегляд параметрів на пристроях.</span><span class="sxs-lookup"><span data-stu-id="7b40f-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="7b40f-115">**Примітка.** Відображення даних звітування для базових планів із початкового розгортання на пристрій може тривати до 24 годин, а подальші оновлення – до 6 годин.</span><span class="sxs-lookup"><span data-stu-id="7b40f-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="7b40f-116">Найпоширеніша причина незастосування параметра базового плану полягає в тому, що параметр використовується в іншому профілі.</span><span class="sxs-lookup"><span data-stu-id="7b40f-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="7b40f-117">Цей сценарій можна дослідити для певного пристрою, вибравши його в вузлі "Стан пристрою" профілю "Базовий план безпеки".</span><span class="sxs-lookup"><span data-stu-id="7b40f-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="7b40f-118">Докладні відомості див. [в статті Усунення конфліктів для базових планів безпеки.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="7b40f-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>