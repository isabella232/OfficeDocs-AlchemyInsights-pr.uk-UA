---
title: Віддалене вирішення проблем із пристроями переходу для Windows 10 для захисту від досвідчених загроз Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750047"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="3dc61-102">Віддалене вирішення проблем із пристроями переходу для Windows 10 для захисту від досвідчених загроз Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="3dc61-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="3dc61-103">Якщо ви можете отримати доступ до віддаленого комп'ютера, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="3dc61-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="3dc61-104">Завантажте засіб діагностики засобу [аналізу підключення клієнта](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="3dc61-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="3dc61-105">Розпакуйте та запустіть програму MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="3dc61-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="3dc61-106">Знайдіть журнал діагностики в папці Mdatpdreclireрезультуючий, що є тією самою папкою, де завантажувалася засіб аналізу.</span><span class="sxs-lookup"><span data-stu-id="3dc61-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="3dc61-107">Щоб отримати проблеми з настройками підключення або проксі-сервера Інтернету, ознайомтеся з файлом журналу MDATPClientAnalyzer.txt.</span><span class="sxs-lookup"><span data-stu-id="3dc61-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="3dc61-108">Щоб дізнатися більше, ознайомтеся [з проблемами з переходу машини](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="3dc61-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
