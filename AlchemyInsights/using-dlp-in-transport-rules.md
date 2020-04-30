---
title: Використання DLP в правилах транспортування
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915299"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="08e0c-102">Використання DLP в правилах транспортування</span><span class="sxs-lookup"><span data-stu-id="08e0c-102">Using DLP in transport rules</span></span>

<span data-ttu-id="08e0c-103">Щоб інтегрувати засіб захисту від втрати даних (DLP) у наявний транспорт, скористайтеся умовою "**Якщо повідомлення містить…Делікатну інформацію**" в параметрі правил транспортування.</span><span class="sxs-lookup"><span data-stu-id="08e0c-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="08e0c-104">**Докладні відомості див. в статті:**</span><span class="sxs-lookup"><span data-stu-id="08e0c-104">**For more details, see:**</span></span>

- <span data-ttu-id="08e0c-105">Інтегровані типи делікатної інформації DLP в правилах транспортування: [Інтегрування правил делікатної інформації](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="08e0c-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="08e0c-106">Крім того, ви можете перевірити правило разом із перевіркою політики або без неї, використовуючи тестовий режим для правила.</span><span class="sxs-lookup"><span data-stu-id="08e0c-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="08e0c-107">Перш ніж перевірити правило, слід почекати 30 хвилин із моменту його створення.</span><span class="sxs-lookup"><span data-stu-id="08e0c-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="08e0c-108">Див. статтю [Перевірка правил передавання пошти (правил транспортування)](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="08e0c-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="08e0c-109">**Примітка.**. Якщо ви намагаєтеся впровадити нову політику DLP за допомогою правил транспортування в EAC, радимо скористатися [політиками DLP в Центрі безпеки та відповідності](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="08e0c-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
