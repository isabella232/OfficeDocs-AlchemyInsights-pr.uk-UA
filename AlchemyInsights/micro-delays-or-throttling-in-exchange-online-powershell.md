---
title: Мікрозатримки та дроселювання в Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702147"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="a649b-102">Мікрозатримки та дроселювання в Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a649b-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="a649b-103">Під час запуску сценаріїв і командлетів в Exchange Online можуть виникати затримки або відображатися попередження "Застосовано мікрозатримку".</span><span class="sxs-lookup"><span data-stu-id="a649b-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="a649b-104">Нижче наведено кілька порад, як вирішити цю проблему.</span><span class="sxs-lookup"><span data-stu-id="a649b-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="a649b-105">Запустіть нашу діагностику, щоб розслабити політики дроселювання PowerShell свого клієнта.</span><span class="sxs-lookup"><span data-stu-id="a649b-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="a649b-106">Це рішення дасть вам найбільше вирішувати проблему.</span><span class="sxs-lookup"><span data-stu-id="a649b-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="a649b-107">Якщо проблему все одно не вдалося вирішити, скористайтеся [модулем PowerShell Exchange Online v2,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)до якого входять командлети на основі REST API, які значно більші.</span><span class="sxs-lookup"><span data-stu-id="a649b-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="a649b-108">Це рішення може чудово підійти для багатьох командлетів Get-, що часто використовуються.</span><span class="sxs-lookup"><span data-stu-id="a649b-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="a649b-109">Якщо потрібно використовувати командлети, які не описано в модулі v2, див. статті Запуск [командлетів PowerShell](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)для великої кількості користувачів у програмі Office 365, у яких йдеться про те, як обійти обмеження дроселювання PowerShell у Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="a649b-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
