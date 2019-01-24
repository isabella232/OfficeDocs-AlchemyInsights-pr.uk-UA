---
title: Моніторинг умовного доступу
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495357"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="bf13e-102">Моніторинг умовного доступу</span><span class="sxs-lookup"><span data-stu-id="bf13e-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="bf13e-p101">Користувачі націлено на умовного доступу будуть отримувати повідомлення по електронній пошті, якщо вони не відповідають вимогам доступ до вашої організації. Щоб вирішити, ми рекомендуємо одну або кілька з таких рішень:</span><span class="sxs-lookup"><span data-stu-id="bf13e-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="bf13e-p102">Якщо пристрій, як припускають, повинен бути, повідомити користувача зайти на портал компанії app і переконайтеся, що він з'являється на порталі компанії. Якщо цього не відбувається, користувач повинен зареєструвати пристрою.</span><span class="sxs-lookup"><span data-stu-id="bf13e-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="bf13e-p103">Блакитні на порталі перейдіть на **Intune \> пристрій дотримання**. У розділі **монітор** натисніть **пристрій відповідності**. Переглянути ваш пристрій дотримання звіту для перевірки пристрою користувача буде позначено як сумісні.</span><span class="sxs-lookup"><span data-stu-id="bf13e-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="bf13e-p104">Блакитні на порталі перейдіть на **Intune \> пристрій дотримання**. У розділі **керування**клацніть **політику**. У списку дотримання політики перевірте, чи профіль призначається для вашого користувача пристрою. Якщо немає профілю присвоюється, потім Intune не буде може підтвердити відповідність стану пристрою.</span><span class="sxs-lookup"><span data-stu-id="bf13e-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="bf13e-114">Редагування поступки умовного доступу користувача.</span><span class="sxs-lookup"><span data-stu-id="bf13e-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="bf13e-115">Блакитні на порталі перейдіть на **Intune \> умовного доступу \> політики**</span><span class="sxs-lookup"><span data-stu-id="bf13e-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="bf13e-116">Виберіть політику зі списку</span><span class="sxs-lookup"><span data-stu-id="bf13e-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="bf13e-117">Виберіть пункт **користувачі та групи**</span><span class="sxs-lookup"><span data-stu-id="bf13e-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="bf13e-p105">Цільової певні політики на кого-то, додати їх до списку **включень** . Щоб переконатися, що людина опускається, є політики, додайте їх до списку **виключити** .</span><span class="sxs-lookup"><span data-stu-id="bf13e-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="bf13e-120">Читати далі: [як пристрої монітор умовного доступу](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="bf13e-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

