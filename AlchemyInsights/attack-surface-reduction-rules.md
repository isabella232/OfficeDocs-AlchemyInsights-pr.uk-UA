---
title: Правила зменшення поверхні атаки
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676569"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="4d821-102">Правила зменшення поверхні атаки</span><span class="sxs-lookup"><span data-stu-id="4d821-102">Attack surface reduction rules</span></span>

<span data-ttu-id="4d821-103">Виключаючи файли або папки, можна серйозно зменшити захист, передбачений правилами зменшення поверхні атаки.</span><span class="sxs-lookup"><span data-stu-id="4d821-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="4d821-104">Файли, які заблокував би правило, дозволено запускати, і звіти або події не записуються.</span><span class="sxs-lookup"><span data-stu-id="4d821-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="4d821-105">Виняток поширюється на всі правила, які дозволяють винятки.</span><span class="sxs-lookup"><span data-stu-id="4d821-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="4d821-106">Виключення ASR використовують такий самий синтаксис, як Антивірус для Microsoft Defender винятки.</span><span class="sxs-lookup"><span data-stu-id="4d821-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="4d821-107">Докладні відомості [див. в Антивірус для Microsoft Defender перевірки винятків.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="4d821-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="4d821-108">Щоб уникнути проблем, перегляньте типові помилки, яких слід уникати під час визначення [винятків.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="4d821-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="4d821-109">Винятки підтримуються не в усіх правилах ASR.</span><span class="sxs-lookup"><span data-stu-id="4d821-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="4d821-110">Щоб перевірити, чи підтримує правило винятки, див. таблицю Правила зменшення поверхні [атаки](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="4d821-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="4d821-111">Правила зменшення поверхні атаки</span><span class="sxs-lookup"><span data-stu-id="4d821-111">Attack surface reduction rules</span></span>

<span data-ttu-id="4d821-112">Поверхня атаки вашої організації включає в себе всі місця, де зловмисник може компромісувати пристрої або мережі організації.</span><span class="sxs-lookup"><span data-stu-id="4d821-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="4d821-113">Зменшення поверхні атаки означає захист пристроїв і мережі організації, що залишає зловмисників меншою кількості способів виконання атак.</span><span class="sxs-lookup"><span data-stu-id="4d821-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="4d821-114">Може допомогти налаштувати правила зменшення поверхні атаки в Microsoft Defender для кінцевої точки.</span><span class="sxs-lookup"><span data-stu-id="4d821-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="4d821-115">Докладні відомості:</span><span class="sxs-lookup"><span data-stu-id="4d821-115">For more information, see:</span></span>

- [<span data-ttu-id="4d821-116">Зіставлення GUID правила ASR з іменем</span><span class="sxs-lookup"><span data-stu-id="4d821-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="4d821-117">Вимоги до правил asR:</span><span class="sxs-lookup"><span data-stu-id="4d821-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="4d821-118">Windows 10 Pro версії 1709 або пізнішої</span><span class="sxs-lookup"><span data-stu-id="4d821-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="4d821-119">Windows 10 Enterprise версії 1709 або пізнішої</span><span class="sxs-lookup"><span data-stu-id="4d821-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="4d821-120">Windows Server, версія 1803 (щопіврічний канал оновлення) або пізніша</span><span class="sxs-lookup"><span data-stu-id="4d821-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="4d821-121">Визначення правильного винятку для застосування</span><span class="sxs-lookup"><span data-stu-id="4d821-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="4d821-122">Знайдіть ідентифікатор події 1121 або 1122 в журналі Microsoft-Windows-Захисник Windows/Operational.</span><span class="sxs-lookup"><span data-stu-id="4d821-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="4d821-123">Оцініться сценарій блокування та контекст і переконайтеся, що цей сценарій потрібно розблокувати.</span><span class="sxs-lookup"><span data-stu-id="4d821-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="4d821-124">Прочитайте значення Шлях у докладних відомостей про подію ( це значення, яке визначає виняток).</span><span class="sxs-lookup"><span data-stu-id="4d821-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="4d821-125">Зробіть виняток якомога строгим.</span><span class="sxs-lookup"><span data-stu-id="4d821-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="4d821-126">За потреби застосуйте символ узагальлення (наприклад, замінити змінну користувача).</span><span class="sxs-lookup"><span data-stu-id="4d821-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="4d821-127">Застосуйте винятки відповідно до своїх потреб у розгортанні.</span><span class="sxs-lookup"><span data-stu-id="4d821-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="4d821-128">Докладні відомості див. в [розділі Налаштування правил зменшення поверхні атаки](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="4d821-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="4d821-129">Виняток не дотримується</span><span class="sxs-lookup"><span data-stu-id="4d821-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="4d821-130">Визначте, чи підтримує правило винятки.</span><span class="sxs-lookup"><span data-stu-id="4d821-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="4d821-131">Докладні відомості див. в [правилах зменшення поверхні атаки](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="4d821-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="4d821-132">Перегляньте винятки, що застосовуються, і перевірте, чи введено неправильно введені або неправильно інтерпретовані символи узагальнення.</span><span class="sxs-lookup"><span data-stu-id="4d821-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="4d821-133">Докладні відомості див. в [розділах Підтримувані типи винятку](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="4d821-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="4d821-134">якщо вплив правила воно задовге, спробуйте перемістити правило (назад) у режим перевірки, щоб виконати подальшу перевірку.</span><span class="sxs-lookup"><span data-stu-id="4d821-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="4d821-135">Докладні відомості див. в [статті Перевірка роботи функцій кінцевої точки в](/microsoft-365/security/defender-endpoint/audit-windows-defender)Microsoft Defender в режимі аудиту.</span><span class="sxs-lookup"><span data-stu-id="4d821-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="4d821-136">Зберіть дані служби підтримки, щоб відкрити інцидент служби підтримки за допомогою цієї команди:</span><span class="sxs-lookup"><span data-stu-id="4d821-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="4d821-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="4d821-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="4d821-138">Докладні відомості див. в статті Проблеми з приєднуванням [до Захисника Microsoft Для кінцевих точок.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="4d821-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
