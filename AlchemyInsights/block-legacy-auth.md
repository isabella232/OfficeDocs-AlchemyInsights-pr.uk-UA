---
title: BlockLegacyAuth
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820199"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="f37ab-102">Блокування застарілої автентифікації</span><span class="sxs-lookup"><span data-stu-id="f37ab-102">Blocking legacy authentication</span></span>

<span data-ttu-id="f37ab-103">Застаріла автентифікація – це термін, який посилається на запит автентифікації, який здійснюються:</span><span class="sxs-lookup"><span data-stu-id="f37ab-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="f37ab-104">Старі клієнти Office, які не використовують сучасну автентифікацію (наприклад, клієнт Office 2010).</span><span class="sxs-lookup"><span data-stu-id="f37ab-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="f37ab-105">Клієнт, який використовує застарілі протоколи пошти, як-от IMAP або SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="f37ab-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="f37ab-106">Докладні відомості про блокування застарілої автентифікації та ввімкнення сучасної автентифікації див. в розділі Блокування [застарілої автентифікації.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="f37ab-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="f37ab-107">Стандартні параметри безпеки в Azure Active Directory (Azure AD) спрощують захист і захист організації.</span><span class="sxs-lookup"><span data-stu-id="f37ab-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="f37ab-108">Стандартні параметри безпеки містять попередньо настроєні параметри безпеки для поширених атак.</span><span class="sxs-lookup"><span data-stu-id="f37ab-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="f37ab-109">Докладні відомості про стандартні параметри безпеки див. в цьому [документі.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="f37ab-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="f37ab-110">**Примітка.** Якщо ваш клієнта створено 22 жовтня 2019 р. або після неї, імовірно, ви за замовчуванням почнете нову поведінку, захищену за замовчуванням, і в клієнта вже активовано стандартні параметри безпеки.</span><span class="sxs-lookup"><span data-stu-id="f37ab-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="f37ab-111">Щоб захистити всіх користувачів, параметри безпеки буде розгорнуто для всіх нових клієнтів.</span><span class="sxs-lookup"><span data-stu-id="f37ab-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
