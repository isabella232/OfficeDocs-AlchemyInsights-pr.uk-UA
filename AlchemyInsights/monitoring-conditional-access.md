---
title: Моніторинг умовного доступу
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713739"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="29e6a-102">Моніторинг умовного доступу для Exchange</span><span class="sxs-lookup"><span data-stu-id="29e6a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="29e6a-103">Користувачі, націлені з умовним доступом, отримають сповіщення електронною поштою, якщо вони не відповідають вимогам до вашої організації.</span><span class="sxs-lookup"><span data-stu-id="29e6a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="29e6a-104">Щоб вирішити проблему, рекомендовано один або кілька таких рішень:</span><span class="sxs-lookup"><span data-stu-id="29e6a-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="29e6a-105">Якщо пристрій передбачається Зарахованим, порадьте користувачеві перейти до програми порталу компанії і переконатися, що вона з'являється на порталі компанії.</span><span class="sxs-lookup"><span data-stu-id="29e6a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="29e6a-106">Якщо це не так, користувач має зареєструвати пристрій.</span><span class="sxs-lookup"><span data-stu-id="29e6a-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="29e6a-107">На порталі Azure перейдіть до \*\* \> InTune пристрою відповідності\*\*.</span><span class="sxs-lookup"><span data-stu-id="29e6a-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="29e6a-108">У розділі **монітор** натисніть **сумісність пристроїв**.</span><span class="sxs-lookup"><span data-stu-id="29e6a-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="29e6a-109">Перегляньте звіт про відповідність пристрою, щоб перевірити, чи пристрій користувача позначено як сумісний.</span><span class="sxs-lookup"><span data-stu-id="29e6a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="29e6a-110">На порталі Azure перейдіть до \*\* \> InTune пристрою відповідності\*\*.</span><span class="sxs-lookup"><span data-stu-id="29e6a-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="29e6a-111">У розділі **керування**виберіть пункт **політики**.</span><span class="sxs-lookup"><span data-stu-id="29e6a-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="29e6a-112">У списку політики дотримання переконайтеся, що профіль призначено для пристрою користувача.</span><span class="sxs-lookup"><span data-stu-id="29e6a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="29e6a-113">Якщо жоден профіль не призначається, то InTune не зможе підтвердити статус відповідності пристрою.</span><span class="sxs-lookup"><span data-stu-id="29e6a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="29e6a-114">Змінити призначення умовного доступу користувача.</span><span class="sxs-lookup"><span data-stu-id="29e6a-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="29e6a-115">На порталі Azure перейти до **InTune \> умовного доступу \> політики**</span><span class="sxs-lookup"><span data-stu-id="29e6a-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="29e6a-116">Виберіть політику зі списку</span><span class="sxs-lookup"><span data-stu-id="29e6a-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="29e6a-117">Натисніть **користувачі та групи**</span><span class="sxs-lookup"><span data-stu-id="29e6a-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="29e6a-118">Щоб націлити користувача на певну політику, додайте їх до списку **включити** .</span><span class="sxs-lookup"><span data-stu-id="29e6a-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="29e6a-119">Щоб переконатися, що користувач пропущено з політики, додайте їх до списку **винятків** .</span><span class="sxs-lookup"><span data-stu-id="29e6a-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="29e6a-120">Докладніше: [як відстежувати пристрої умовного доступу](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="29e6a-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

