---
title: Використання DLP в правилах транспортування
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
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827237"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="4747a-102">Використання DLP в правилах транспортування</span><span class="sxs-lookup"><span data-stu-id="4747a-102">Using DLP in transport rules</span></span>

<span data-ttu-id="4747a-103">Щоб інтегрувати засіб захисту від втрати даних (DLP) у наявний транспорт, скористайтеся умовою "**Якщо повідомлення містить…Делікатну інформацію**" в параметрі правил транспортування.</span><span class="sxs-lookup"><span data-stu-id="4747a-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="4747a-104">**Докладні відомості див. в статті:**</span><span class="sxs-lookup"><span data-stu-id="4747a-104">**For more details, see:**</span></span>

- <span data-ttu-id="4747a-105">Інтегровані типи делікатної інформації DLP в правилах транспортування: [Інтегрування правил делікатної інформації](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="4747a-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="4747a-106">Крім того, ви можете перевірити правило разом із перевіркою політики або без неї, використовуючи тестовий режим для правила.</span><span class="sxs-lookup"><span data-stu-id="4747a-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="4747a-107">Перш ніж перевірити правило, слід почекати 30 хвилин із моменту його створення.</span><span class="sxs-lookup"><span data-stu-id="4747a-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="4747a-108">Див. статтю [Перевірка правил передавання пошти (правил транспортування)](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="4747a-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="4747a-109">**Примітка.**. Якщо ви намагаєтеся впровадити нову політику DLP за допомогою правил транспортування в EAC, радимо скористатися [політиками DLP в Центрі безпеки та відповідності](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="4747a-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
