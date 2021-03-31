---
title: EndPoint Manager – базові плани безпеки
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440914"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="7ca97-102">EndPoint Manager – базові плани безпеки</span><span class="sxs-lookup"><span data-stu-id="7ca97-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="7ca97-103">Базові плани безпеки – це попередньо налаштовані групи параметрів Windows, які допомагають застосувати параметри безпеки, рекомендовані відповідними групами безпеки.</span><span class="sxs-lookup"><span data-stu-id="7ca97-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="7ca97-104">Ці базові плани можна настроїти так, щоб вони постачали лише бажані параметри та значення.</span><span class="sxs-lookup"><span data-stu-id="7ca97-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="7ca97-105">Докладні відомості про базові плани безпеки див. в статті [Використання базових планів безпеки для настроювання пристроїв із Windows 10 в Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="7ca97-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="7ca97-106">Наразі є базові плани для цих продуктів:</span><span class="sxs-lookup"><span data-stu-id="7ca97-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="7ca97-107">Параметри безпеки MDM у Windows</span><span class="sxs-lookup"><span data-stu-id="7ca97-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="7ca97-108">Безпека Microsoft Defender для кінцевих точок</span><span class="sxs-lookup"><span data-stu-id="7ca97-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="7ca97-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="7ca97-109">Microsoft Edge</span></span>

<span data-ttu-id="7ca97-110">Кожен із базових планів періодично оновлюється та випускається в інкрементних версіях.</span><span class="sxs-lookup"><span data-stu-id="7ca97-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="7ca97-111">Кожна версія додає та видаляє параметри з попередньої версії, щоб забезпечити відповідність базового плану поточним рекомендаціям.</span><span class="sxs-lookup"><span data-stu-id="7ca97-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="7ca97-112">Консоль безпеки базового плану для кінцевих точок дає змогу порівняти різні версії, показуючи зміни з версії до версії.</span><span class="sxs-lookup"><span data-stu-id="7ca97-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="7ca97-113">Докладні відомості про те, як ефективніше змінити версію застосованого базового плану, див. в статті [Налаштування профілів базового плану безпеки в Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="7ca97-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="7ca97-114">Розгорнувши базовий план безпеки, можна відстежувати стан розгортання та переглядати параметри для кожного пристрою.</span><span class="sxs-lookup"><span data-stu-id="7ca97-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="7ca97-115">**Примітка:** Дані звітування для базових планів можуть з'явитися протягом 24 годин від початкового розгортання для пристрою та до 6 годин для подальших оновлень.</span><span class="sxs-lookup"><span data-stu-id="7ca97-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="7ca97-116">Найпоширеніша причина незастосованого параметра базового плану полягає в тому, що той самий параметр використовується в іншому профілі.</span><span class="sxs-lookup"><span data-stu-id="7ca97-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="7ca97-117">Цей сценарій можна дослідити для певного пристрою, вибравши його у вузлі "Стан пристрою" профілю базового плану безпеки.</span><span class="sxs-lookup"><span data-stu-id="7ca97-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="7ca97-118">Докладні відомості див. [Вирішення конфліктів для базових планів безпеки](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="7ca97-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>