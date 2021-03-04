---
title: Помилки синхронізації автоматичної реєстрації пристрою в Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448943"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="27342-102">Помилки синхронізації автоматичної реєстрації пристрою в Apple</span><span class="sxs-lookup"><span data-stu-id="27342-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="27342-103">"Виявлено, що у вас є один або кілька маркерів ADE/DEP, які знаходяться в стані помилки.</span><span class="sxs-lookup"><span data-stu-id="27342-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="27342-104">Доки стан помилки не буде вирішено для кожного відповідного маркера, функція ADE не працюватиме належним чином. ".</span><span class="sxs-lookup"><span data-stu-id="27342-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="27342-105">Ця помилка може виявлятися кількома способами, зокрема:</span><span class="sxs-lookup"><span data-stu-id="27342-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="27342-106">Пристрої можуть не синхронізуватися з ABM/ASM для Inune</span><span class="sxs-lookup"><span data-stu-id="27342-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="27342-107">Можливо, не вдається отримати відповідні завдання для реєстрації</span><span class="sxs-lookup"><span data-stu-id="27342-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="27342-108">Можливо, для пристроїв не вдалося завершити реєстрацію в "ADE"</span><span class="sxs-lookup"><span data-stu-id="27342-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="27342-109">Перевірте, чи повідомлення про помилку синхронізації повідомляється в консолі Inune в розділі **пристрої, > записатися на пристрої > програми реєстрації в програмі Apple > маркери для реєстрації**.</span><span class="sxs-lookup"><span data-stu-id="27342-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="27342-110">Однією з найпоширеніших причин помилки синхронізації є термін дії поточного маркера.</span><span class="sxs-lookup"><span data-stu-id="27342-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="27342-111">У багатьох випадках відновлення ураженого маркера вирішить проблему.</span><span class="sxs-lookup"><span data-stu-id="27342-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="27342-112">Якщо термін дії одного або кількох маркерів минув, ознайомтеся з наведеною нижче документацією, щоб допомогти вам поновити їх відповідно до таких потреб:</span><span class="sxs-lookup"><span data-stu-id="27342-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="27342-113">Поновлення маркера реєстрації автоматичного пристрою</span><span class="sxs-lookup"><span data-stu-id="27342-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="27342-114">Крім того, можна переглянути наведені нижче документи, щоб переглянути потенційні помилки для інших помилок, які призводять до помилок синхронізації маркерів.</span><span class="sxs-lookup"><span data-stu-id="27342-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="27342-115">Помилки синхронізації АБМ/АНМ для маркерів реєстрації для iOS/iPadOS і macOS для автоматичних пристроїв</span><span class="sxs-lookup"><span data-stu-id="27342-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="27342-116">Помилки синхронізації АБМ/АНМ для маркерів реєстрації для iOS/iPadOS і macOS для автоматичних пристроїв</span><span class="sxs-lookup"><span data-stu-id="27342-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
