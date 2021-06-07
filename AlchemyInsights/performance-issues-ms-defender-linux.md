---
title: Проблеми з продуктивністю кінцевої точки для Захисника Microsoft у Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794222"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="dd90a-102">Проблеми з продуктивністю кінцевої точки для Захисника Microsoft у Linux</span><span class="sxs-lookup"><span data-stu-id="dd90a-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="dd90a-103">У цій статті описано кроки з визначення проблем із продуктивністю для кінцевої точки Microsoft Defender у Linux.</span><span class="sxs-lookup"><span data-stu-id="dd90a-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="dd90a-104">Спочатку переконайтеся, що проблему, з якою виникла проблема, вирішено в найновішій [версії](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span><span class="sxs-lookup"><span data-stu-id="dd90a-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="dd90a-105">Відомості про початок дослідження див. в статті Усунення несправностей із продуктивністю [microsoft Defender для кінцевої точки в Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="dd90a-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="dd90a-106">Винятки</span><span class="sxs-lookup"><span data-stu-id="dd90a-106">Exclusions</span></span>

<span data-ttu-id="dd90a-107">Винятки можуть допомогти знизити продуктивність.</span><span class="sxs-lookup"><span data-stu-id="dd90a-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="dd90a-108">Перш ніж почати, перегляньте винятки, щоб отримати додаткову інформацію про ризик і документацію.</span><span class="sxs-lookup"><span data-stu-id="dd90a-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="dd90a-109">Докладні відомості див. в статті Налаштування та перевірка винятків для Microsoft [Defender для кінцевої точки в Linux.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="dd90a-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="dd90a-110">Якщо у вас є кілька файлів & папок, які потрібно виключити, і всі вони на одній горині, може бути легше виключити байт.</span><span class="sxs-lookup"><span data-stu-id="dd90a-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="dd90a-111">Починаючи з лютого випуску 101.22.80, ви можете виключити всю точку встановлення.</span><span class="sxs-lookup"><span data-stu-id="dd90a-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="dd90a-112">Наприклад, якщо /mnt/backup – це байтна точка, до списку виключених елементів можна додати /mnt/backup, запустивши таку команду:</span><span class="sxs-lookup"><span data-stu-id="dd90a-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="dd90a-113">**Примітка.** Додавання винятків підвищує ризик того, що зловмисне програмне забезпечення не виявляється, і його потрібно обробляти та впроваджувати з обережністю.</span><span class="sxs-lookup"><span data-stu-id="dd90a-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="dd90a-114">Потрібна допомога?</span><span class="sxs-lookup"><span data-stu-id="dd90a-114">Need Help?</span></span>

<span data-ttu-id="dd90a-115">Щоб допомогти вам у найефективнішому способі, зберіть діагностичні дані, перш ніж відкривати інцидент служби підтримки.</span><span class="sxs-lookup"><span data-stu-id="dd90a-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
