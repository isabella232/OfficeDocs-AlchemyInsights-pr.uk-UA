---
title: Проблеми з приєднанням комп'ютерів до Microsoft Defender для кінцевих точок
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 7ccec69f8ab43f277978176519a7f8f8df443846
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "50901588"
---
# <a name="issues-with-onboarding-machines-to-microsoft-defender-for-endpoints"></a><span data-ttu-id="04a51-102">Проблеми з приєднанням комп'ютерів до Microsoft Defender для кінцевих точок</span><span class="sxs-lookup"><span data-stu-id="04a51-102">Issues with onboarding machines to Microsoft Defender for Endpoints</span></span>

<span data-ttu-id="04a51-103">У вас можуть виникнути проблеми з приєднанням комп'ютерів до служби MDE.</span><span class="sxs-lookup"><span data-stu-id="04a51-103">You might have issues with onboarding machines to MDE service.</span></span> <span data-ttu-id="04a51-104">Якщо ви можете отримати доступ до комп'ютера користувача, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="04a51-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="04a51-105">Завантажте останню ознайомлювальну версію інструменту діагностики[MDE Client Analyzer](https://aka.ms/betamdeanalyzer).</span><span class="sxs-lookup"><span data-stu-id="04a51-105">Download the latest preview version of the [MDE Client Analyzer](https://aka.ms/betamdeanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="04a51-106">Клацніть правою кнопкою **MDEClientAnalyzer.cmd** і виберіть пункт "Запуск із правами адміністратора".</span><span class="sxs-lookup"><span data-stu-id="04a51-106">Right click **MDEClientAnalyzer.cmd** and select ‘Run as administrator’.</span></span>
3. <span data-ttu-id="04a51-107">Дотримуйтеся вказівок, запропонованих у **MDEClientAnalyzer.htm**.</span><span class="sxs-lookup"><span data-stu-id="04a51-107">Follow any guidance suggested in **MDEClientAnalyzer.htm**.</span></span>
4. <span data-ttu-id="04a51-108">Докладніші журнали можна подивитися у створеній вкладеній папці з ім'ям **MDEClientAnalyzerResult**.</span><span class="sxs-lookup"><span data-stu-id="04a51-108">For more verbose logs, review the created sub-folder named **MDEClientAnalyzerResult**.</span></span>
5. <span data-ttu-id="04a51-109">Якщо вам потрібні додаткові інструкції, зверніться до [служби підтримки Microsoft Defender для кінцевих точок](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) і надішліть отриманий файл MDEClientAnalyzerResult.zip для аналізу.</span><span class="sxs-lookup"><span data-stu-id="04a51-109">If additional guidance is needed, contact [Microsoft Defender for Endpoint support](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/contact-support) and provide the resulting MDEClientAnalyzerResult.zip file for analysis.</span></span>
