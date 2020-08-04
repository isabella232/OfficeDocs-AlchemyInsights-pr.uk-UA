---
title: Призупинення запланованих оновлень
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555994"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="db771-102">Призупинення запланованих оновлень</span><span class="sxs-lookup"><span data-stu-id="db771-102">Pausing scheduled updates</span></span>

<span data-ttu-id="db771-103">Після того, як буде випущено команду призупинення, пристрої не обробляти команду до наступного разу, коли вони перевіряють в InTune.</span><span class="sxs-lookup"><span data-stu-id="db771-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="db771-104">У зв'язку з цим ваші пристрої можуть мати:</span><span class="sxs-lookup"><span data-stu-id="db771-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="db771-105">Інстальовано заплановані оновлення до реєстрації.</span><span class="sxs-lookup"><span data-stu-id="db771-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="db771-106">Було вимкнено, коли ви видали команду паузи.</span><span class="sxs-lookup"><span data-stu-id="db771-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="db771-107">У цьому випадку, коли пристрої ввімкнуто, вони могли завантажити та інсталювати заплановані оновлення до реєстрації.</span><span class="sxs-lookup"><span data-stu-id="db771-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>