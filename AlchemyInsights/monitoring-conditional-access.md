---
title: Моніторинг умовного доступу
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708695"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="c2438-102">Моніторинг умовного доступу для Exchange</span><span class="sxs-lookup"><span data-stu-id="c2438-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="c2438-103">Користувачі, які націлені на умовний доступ, отримають сповіщення електронною поштою, якщо вони не відповідатимуть вимогам доступу до вашої організації.</span><span class="sxs-lookup"><span data-stu-id="c2438-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="c2438-104">Щоб вирішити цю проблему, радимо виконати одну або кілька з наведених нижче рішень.</span><span class="sxs-lookup"><span data-stu-id="c2438-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="c2438-105">Якщо пристрій має бути зареєстровано, радимо користувачу перейти до програми "портал компанії" та переконатися, що вона з'явиться на порталі компанії.</span><span class="sxs-lookup"><span data-stu-id="c2438-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="c2438-106">Якщо це не так, користувач має зареєструвати пристрій.</span><span class="sxs-lookup"><span data-stu-id="c2438-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="c2438-107">На порталі "Лазурний" перейдіть на сайт > відповідність пристрою.</span><span class="sxs-lookup"><span data-stu-id="c2438-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="c2438-108">У розділі монітор виберіть елемент відповідність пристрою.</span><span class="sxs-lookup"><span data-stu-id="c2438-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="c2438-109">Перегляньте звіт про відповідність пристрою, щоб переконатися, що пристрій користувача позначено як сумісний.</span><span class="sxs-lookup"><span data-stu-id="c2438-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="c2438-110">На порталі "Лазурний" перейдіть на сайт > відповідність пристрою.</span><span class="sxs-lookup"><span data-stu-id="c2438-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="c2438-111">У розділі керування виберіть елемент політики.</span><span class="sxs-lookup"><span data-stu-id="c2438-111">Under Manage, click Policies.</span></span> <span data-ttu-id="c2438-112">У списку політик відповідності переконайтеся, що профіль призначається для вашого пристрою користувача.</span><span class="sxs-lookup"><span data-stu-id="c2438-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="c2438-113">Якщо не призначено профіль, функція Inune не зможе підтвердити стан відповідності пристрою.</span><span class="sxs-lookup"><span data-stu-id="c2438-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="c2438-114">Редагування призначення умовного доступу користувача.</span><span class="sxs-lookup"><span data-stu-id="c2438-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="c2438-115">На порталі Лазурне **перейдіть до**  >  **політики умовного доступу**, що містяться в службі Access  >  .</span><span class="sxs-lookup"><span data-stu-id="c2438-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="c2438-116">Виберіть політику зі списку.</span><span class="sxs-lookup"><span data-stu-id="c2438-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="c2438-117">Виберіть елемент користувачі та групи.</span><span class="sxs-lookup"><span data-stu-id="c2438-117">Click Users and groups.</span></span>
4. <span data-ttu-id="c2438-118">Щоб націлити певну політику на когось, додайте їх до списку include.</span><span class="sxs-lookup"><span data-stu-id="c2438-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="c2438-119">Щоб переконатися, що особу пропущено від політики, додайте їх до списку винятків.</span><span class="sxs-lookup"><span data-stu-id="c2438-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="c2438-120">Корисні посилання:</span><span class="sxs-lookup"><span data-stu-id="c2438-120">Helpful links:</span></span>

[<span data-ttu-id="c2438-121">Огляд відповідності пристрою</span><span class="sxs-lookup"><span data-stu-id="c2438-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="c2438-122">Виправлення неполадок із CA</span><span class="sxs-lookup"><span data-stu-id="c2438-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="c2438-123">Виправлення неполадок із політикою</span><span class="sxs-lookup"><span data-stu-id="c2438-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="c2438-124">Відстеження відповідності пристрою</span><span class="sxs-lookup"><span data-stu-id="c2438-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="c2438-125">Зверніть увагу, що ці дії доступні лише для виправлення неполадок із умовною доступом до функції "Лазурний".</span><span class="sxs-lookup"><span data-stu-id="c2438-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="c2438-126">Крім того, можна використовувати карантин пристрою, що блокує доступ до електронної пошти з політикою Exchange.</span><span class="sxs-lookup"><span data-stu-id="c2438-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="c2438-127">Додаткові відомості про керування пристроями Exchange можна знайти [тут] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="c2438-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
