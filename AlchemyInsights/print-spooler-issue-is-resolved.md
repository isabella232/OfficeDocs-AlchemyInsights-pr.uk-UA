---
title: Усунуто проблему спулера друку
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/08/2020
ms.locfileid: "45088529"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="13373-102">Усунуто проблему спулера друку</span><span class="sxs-lookup"><span data-stu-id="13373-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="13373-103">Якщо пристрій було оновлено з ОС Windows 10 **OS Build 19041,329**, можливо, спостерігається проблема, коли деякі принтери не друкувати.</span><span class="sxs-lookup"><span data-stu-id="13373-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="13373-104">Спулеру друку може викинути помилку або несподівано закрити під час спроби друку, і вихід із відповідного принтера не надходить.</span><span class="sxs-lookup"><span data-stu-id="13373-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="13373-105">Цю проблему усунуто в ОС збірка **19041,331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span><span class="sxs-lookup"><span data-stu-id="13373-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="13373-106">**Поточне розслідування**</span><span class="sxs-lookup"><span data-stu-id="13373-106">**Ongoing investigation**</span></span>

<span data-ttu-id="13373-107">На деяких пристроях, з повідомленням про помилку, може не вдатися до**Isass.exe**LSASS, а не вдалося виконати на деякі пристрої, "критичний системний процес, C:\WINDOWS\system32\Isass.exe, помилка з кодом стану c0000008".</span><span class="sxs-lookup"><span data-stu-id="13373-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="13373-108">Машина тепер має бути перезапущено ".</span><span class="sxs-lookup"><span data-stu-id="13373-108">The machine must now be restarted".</span></span>  <span data-ttu-id="13373-109">**Корпорація Майкрософт працює над роздільною здатністю та надасть оновлення в майбутньому випуску.**</span><span class="sxs-lookup"><span data-stu-id="13373-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="13373-110">Щоб отримати додаткові відомості, будь ласка, ознайомтеся з [Windows 10 версії 2004 відомі проблеми](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span><span class="sxs-lookup"><span data-stu-id="13373-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>