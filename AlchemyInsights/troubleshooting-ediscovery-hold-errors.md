---
title: Виправлення помилок служби ediscovery
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676531"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="00307-102">Виправлення помилок служби ediscovery</span><span class="sxs-lookup"><span data-stu-id="00307-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="00307-103">Виникли проблеми з утриманням витребування електронної даних?</span><span class="sxs-lookup"><span data-stu-id="00307-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="00307-104">Нижче наведено кілька порад, які слід врахувати.</span><span class="sxs-lookup"><span data-stu-id="00307-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="00307-105">Перевірте стан розподілу утримання.</span><span class="sxs-lookup"><span data-stu-id="00307-105">Check the hold distribution status.</span></span>  <span data-ttu-id="00307-106">Якщо стан **Увімкнуто (очікує)** або Вимк. **(Очікує),** зачекайте, доки не завершиться розподіл утримання.</span><span class="sxs-lookup"><span data-stu-id="00307-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="00307-107">Об'єднайте оновлення для витребування електронної інформації, щоб проводити оновлення в один груповий запит, а не постійно оновлювати політику для кожної транзакції.</span><span class="sxs-lookup"><span data-stu-id="00307-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="00307-108">Запустіть Set-CaseHoldPolicy <policyname> -RetryDistribution в PowerShell Центру безпеки та відповідності.</span><span class="sxs-lookup"><span data-stu-id="00307-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="00307-109">Докладні відомості [див. в Підключення PowerShell & безпеки та відповідності.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="00307-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="00307-110">Указівки з перевірки цих параметрів і додаткові практичні поради з виправлення неполадок утримання витребування електронної пошти див. в цій [статті.](/microsoft-365/compliance/hold-distribution-errors)</span><span class="sxs-lookup"><span data-stu-id="00307-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="00307-111">Відомості про виправлення інших поширених проблем витребування електронної інформації див. в розділах Дослідження, усунення несправностей і вирішення поширених проблем витребування [електронної інформації.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="00307-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
