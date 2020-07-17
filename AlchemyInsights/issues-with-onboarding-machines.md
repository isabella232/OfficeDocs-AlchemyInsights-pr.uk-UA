---
title: Проблеми з машинами для ознайомлення
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141839"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="2029e-102">Проблеми з машинами для ознайомлення</span><span class="sxs-lookup"><span data-stu-id="2029e-102">Issues with onboarding machines</span></span>

<span data-ttu-id="2029e-103">Можливо, виникли проблеми з машинами для ознайомлення з службою MDATP.</span><span class="sxs-lookup"><span data-stu-id="2029e-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="2029e-104">Якщо ви можете отримати доступ до машини кінцевого користувача, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="2029e-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="2029e-105">Завантажити засіб діагностики [підключення до клієнта](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="2029e-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="2029e-106">Розпакуйте і запустіть MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="2029e-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="2029e-107">Знайдіть журнал діагностики в папці Mdatpклієнтаналізрезультат, ту саму папку, де завантажується засіб аналізатора.</span><span class="sxs-lookup"><span data-stu-id="2029e-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="2029e-108">Перегляньте файл журналу MDATPClientAnalyzer.txt, щоб знайти настройки підключення до Інтернету або проксі-сервера.</span><span class="sxs-lookup"><span data-stu-id="2029e-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>