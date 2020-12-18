---
title: Помилки синхронізації автоматичної реєстрації пристрою в Apple
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714971"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="5647c-102">Помилки синхронізації автоматичної реєстрації пристрою в Apple</span><span class="sxs-lookup"><span data-stu-id="5647c-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="5647c-103">"Виявлено, що у вас є один або кілька маркерів ADE/DEP, які знаходяться в стані помилки.</span><span class="sxs-lookup"><span data-stu-id="5647c-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="5647c-104">Доки стан помилки не буде вирішено для кожного відповідного маркера, функція ADE не працюватиме для одних і тих самих ".</span><span class="sxs-lookup"><span data-stu-id="5647c-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="5647c-105">Ця помилка може виявлятися кількома способами, зокрема:</span><span class="sxs-lookup"><span data-stu-id="5647c-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="5647c-106">Пристрої можуть не синхронізуватися з ABM/ASM для Inune</span><span class="sxs-lookup"><span data-stu-id="5647c-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="5647c-107">Можливо, не вдається отримати відповідні завдання для реєстрації</span><span class="sxs-lookup"><span data-stu-id="5647c-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="5647c-108">Можливо, для пристроїв не вдалося завершити реєстрацію в "ADE"</span><span class="sxs-lookup"><span data-stu-id="5647c-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="5647c-109">Перевірте, чи повідомлення про помилку синхронізації відобразилось в консолі Inune в розділі **пристрої, > записатися на пристрої > програми реєстрації в програмі Apple >** , а також Перегляньте наведені нижче документи, щоб переглянути потенційні виправлення.</span><span class="sxs-lookup"><span data-stu-id="5647c-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="5647c-110">Помилки синхронізації АБМ/АНМ для маркерів реєстрації для iOS/iPadOS і macOS для автоматичних пристроїв</span><span class="sxs-lookup"><span data-stu-id="5647c-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
