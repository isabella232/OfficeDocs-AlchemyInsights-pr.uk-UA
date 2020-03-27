---
title: Піктограма календаря не відображається в клієнті Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 21692639fb746b2e5aab3dfc8894293d5dc890ac
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932380"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="fffea-102">Піктограма календаря не відображається в клієнті Teams</span><span class="sxs-lookup"><span data-stu-id="fffea-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="fffea-103">Вкладці "Календар" у Teams потрібен доступ до поштової скриньки Exchange через веб-служби Exchange.</span><span class="sxs-lookup"><span data-stu-id="fffea-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="fffea-104">Поштова скринька Exchange може бути онлайновою або локальною.</span><span class="sxs-lookup"><span data-stu-id="fffea-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="fffea-105">Для онлайнових користувачів вкладка "Календар" не відображається. Переконайтеся, що [вони мають ліцензію на поштову скриньку Exchange Online і що поштову скриньку ввімкнуто](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="fffea-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="fffea-106">Якщо користувач має дійсну поштову скриньку в Exchange Online, але вкладка "Календар" не відображається, можливо, виникли неполадки в мережі.</span><span class="sxs-lookup"><span data-stu-id="fffea-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="fffea-107">Скористайтеся [засобом аналізу віддаленого доступу Microsoft Remote](https://testconnectivity.microsoft.com/) і запустіть **перевірку підключення до веб-служб Microsoft Exchange** для користувача, який зазнав впливу.</span><span class="sxs-lookup"><span data-stu-id="fffea-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="fffea-108">Перегляньте [програми Teams (політики налаштування програми)](https://admin.teams.microsoft.com/policies/app-setup), щоб переконатися, що програму "Календар" не вилучено з політики, яка застосовується до користувача (зазвичай **із глобальної політики, яка використовується за замовчуванням для всієї організації**).</span><span class="sxs-lookup"><span data-stu-id="fffea-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="fffea-109">Якщо ваші користувачі перебувають у локальному середовищі, переконайтеся, що гібридна конфігурація справна.</span><span class="sxs-lookup"><span data-stu-id="fffea-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="fffea-110">Щоб вирішити проблему, скористайтеся [майстром гібридної конфігурації](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent).</span><span class="sxs-lookup"><span data-stu-id="fffea-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="fffea-111">Зверніть увагу, що [для Teams необхідно інсталювати Exchange 2016 CU3 або новішої версії](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="fffea-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
