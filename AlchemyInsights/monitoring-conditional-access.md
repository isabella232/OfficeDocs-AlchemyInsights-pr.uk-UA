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
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702924"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="f098b-102">Моніторинг умовного доступу для Exchange</span><span class="sxs-lookup"><span data-stu-id="f098b-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="f098b-103">Користувачі, які націлені на умовний доступ, отримають сповіщення електронною поштою, якщо вони не відповідатимуть вимогам доступу до вашої організації.</span><span class="sxs-lookup"><span data-stu-id="f098b-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="f098b-104">Щоб вирішити цю проблему, радимо виконати одну або кілька з наведених нижче рішень.</span><span class="sxs-lookup"><span data-stu-id="f098b-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="f098b-105">Якщо пристрій має бути зареєстровано, радимо користувачу перейти до програми "портал компанії" та переконатися, що вона з'явиться на порталі компанії.</span><span class="sxs-lookup"><span data-stu-id="f098b-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="f098b-106">Якщо це не так, користувач має зареєструвати пристрій.</span><span class="sxs-lookup"><span data-stu-id="f098b-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="f098b-107">На порталі Лазурне перейдіть до \*\* \> відповідності пристрою inune\*\*.</span><span class="sxs-lookup"><span data-stu-id="f098b-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="f098b-108">У розділі **монітор** виберіть елемент **відповідність пристрою**.</span><span class="sxs-lookup"><span data-stu-id="f098b-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="f098b-109">Перегляньте звіт про відповідність пристрою, щоб переконатися, що пристрій користувача позначено як сумісний.</span><span class="sxs-lookup"><span data-stu-id="f098b-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="f098b-110">На порталі Лазурне перейдіть до \*\* \> відповідності пристрою inune\*\*.</span><span class="sxs-lookup"><span data-stu-id="f098b-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="f098b-111">У розділі **керування**виберіть елемент **політики**.</span><span class="sxs-lookup"><span data-stu-id="f098b-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="f098b-112">У списку політик відповідності переконайтеся, що профіль призначається для вашого пристрою користувача.</span><span class="sxs-lookup"><span data-stu-id="f098b-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="f098b-113">Якщо не призначено профіль, функція Inune не зможе підтвердити стан відповідності пристрою.</span><span class="sxs-lookup"><span data-stu-id="f098b-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="f098b-114">Редагування призначення умовного доступу користувача.</span><span class="sxs-lookup"><span data-stu-id="f098b-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="f098b-115">На порталі "Лазурний" перейдіть до \*\* \> \> політики умовного доступу "inune\*\* "</span><span class="sxs-lookup"><span data-stu-id="f098b-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="f098b-116">Вибір політики зі списку</span><span class="sxs-lookup"><span data-stu-id="f098b-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="f098b-117">Виберіть елемент **користувачі та групи**</span><span class="sxs-lookup"><span data-stu-id="f098b-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="f098b-118">Щоб націлити певну політику на когось, додайте їх до списку **INCLUDE** .</span><span class="sxs-lookup"><span data-stu-id="f098b-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="f098b-119">Щоб переконатися, що особу пропущено від політики, додайте їх до списку **винятків** .</span><span class="sxs-lookup"><span data-stu-id="f098b-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="f098b-120">Докладніше: [відстеження пристроїв умовного доступу](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="f098b-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

