---
title: Відстеження умовного доступу
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428311"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="ced54-102">Відстеження умовного доступу</span><span class="sxs-lookup"><span data-stu-id="ced54-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="ced54-103">Користувачі, які націлені на умовний доступ, отримають сповіщення електронною поштою, якщо вони не відповідатимуть вимогам доступу до вашої організації.</span><span class="sxs-lookup"><span data-stu-id="ced54-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="ced54-104">Щоб вирішити цю проблему, радимо виконати одну або кілька з наведених нижче рішень.</span><span class="sxs-lookup"><span data-stu-id="ced54-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="ced54-105">Якщо пристрій має бути зареєстровано, радимо користувачу перейти до програми "портал компанії" та переконатися, що вона з'явиться на порталі компанії.</span><span class="sxs-lookup"><span data-stu-id="ced54-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="ced54-106">Якщо це не так, користувач має зареєструвати пристрій.</span><span class="sxs-lookup"><span data-stu-id="ced54-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="ced54-107">На порталі Лазурне перейдіть до   >  **відповідності пристрою** inune.</span><span class="sxs-lookup"><span data-stu-id="ced54-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="ced54-108">Щоб переглянути звіт про відповідність пристрою, щоб переконатися, що пристрій користувача позначено як сумісний, у розділі **монітор** виберіть елемент **відповідність пристрою**.</span><span class="sxs-lookup"><span data-stu-id="ced54-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="ced54-109">На порталі Лазурне перейдіть до   >  **відповідності пристрою** inune.</span><span class="sxs-lookup"><span data-stu-id="ced54-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="ced54-110">У розділі **керування** виберіть елемент **політики**.</span><span class="sxs-lookup"><span data-stu-id="ced54-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="ced54-111">У списку політик відповідності переконайтеся, що профіль призначається для вашого пристрою користувача.</span><span class="sxs-lookup"><span data-stu-id="ced54-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="ced54-112">Якщо не призначено профіль, функція Inune не зможе підтвердити стан відповідності пристрою.</span><span class="sxs-lookup"><span data-stu-id="ced54-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="ced54-113">Редагування призначення умовного доступу користувача.</span><span class="sxs-lookup"><span data-stu-id="ced54-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="ced54-114">На порталі "Лазурний" **перейдіть на** вкладку "політики  >  **умовного доступу**  >  ", виберіть політику зі списку, а потім клацніть елемент **користувачі та групи**.</span><span class="sxs-lookup"><span data-stu-id="ced54-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="ced54-115">Щоб націлити певну політику на когось, додайте їх до **списку include**.</span><span class="sxs-lookup"><span data-stu-id="ced54-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="ced54-116">Щоб переконатися, що особу пропущено від політики, додайте їх до **списку винятків**.</span><span class="sxs-lookup"><span data-stu-id="ced54-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="ced54-117">**Корисні посилання:**</span><span class="sxs-lookup"><span data-stu-id="ced54-117">**Helpful links:**</span></span>

- [<span data-ttu-id="ced54-118">Огляд відповідності пристрою</span><span class="sxs-lookup"><span data-stu-id="ced54-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="ced54-119">Виправлення неполадок із CA</span><span class="sxs-lookup"><span data-stu-id="ced54-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="ced54-120">Виправлення неполадок із політикою</span><span class="sxs-lookup"><span data-stu-id="ced54-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="ced54-121">Відстеження відповідності пристрою</span><span class="sxs-lookup"><span data-stu-id="ced54-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="ced54-122">Ці дії доступні лише для виправлення неполадок із умовною доступом до функції "Лазурний".</span><span class="sxs-lookup"><span data-stu-id="ced54-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="ced54-123">Крім того, можна використовувати карантин пристрою, що блокує доступ до електронної пошти з політикою Exchange.</span><span class="sxs-lookup"><span data-stu-id="ced54-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="ced54-124">Додаткові відомості про керування пристроями Exchange можна знайти [**тут**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="ced54-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
