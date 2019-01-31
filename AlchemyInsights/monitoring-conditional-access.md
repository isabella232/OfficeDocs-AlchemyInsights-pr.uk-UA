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
ms.openlocfilehash: f4153f8a87a138d548c133142b0d48a319bd4b71
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656588"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="c3366-102">Моніторинг умовного доступу</span><span class="sxs-lookup"><span data-stu-id="c3366-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="c3366-p101">Користувачі націлено на умовного доступу будуть отримувати повідомлення по електронній пошті, якщо вони не відповідають вимогам доступ до вашої організації. Щоб вирішити, ми рекомендуємо одну або кілька з таких рішень:</span><span class="sxs-lookup"><span data-stu-id="c3366-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="c3366-p102">Якщо пристрій, як припускають, повинен бути, повідомити користувача зайти на портал компанії app і переконайтеся, що він з'являється на порталі компанії. Якщо цього не відбувається, користувач повинен зареєструвати пристрою.</span><span class="sxs-lookup"><span data-stu-id="c3366-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="c3366-p103">Блакитні на порталі перейдіть на **Intune \> пристрій дотримання**. У розділі **монітор** натисніть **пристрій відповідності**. Переглянути ваш пристрій дотримання звіту для перевірки пристрою користувача буде позначено як сумісні.</span><span class="sxs-lookup"><span data-stu-id="c3366-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="c3366-p104">Блакитні на порталі перейдіть на **Intune \> пристрій дотримання**. У розділі **керування**клацніть **політику**. У списку дотримання політики перевірте, чи профіль призначається для вашого користувача пристрою. Якщо немає профілю присвоюється, потім Intune не буде може підтвердити відповідність стану пристрою.</span><span class="sxs-lookup"><span data-stu-id="c3366-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="c3366-114">Редагування поступки умовного доступу користувача.</span><span class="sxs-lookup"><span data-stu-id="c3366-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="c3366-115">Блакитні на порталі перейдіть на **Intune \> умовного доступу \> політики**</span><span class="sxs-lookup"><span data-stu-id="c3366-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="c3366-116">Виберіть політику зі списку</span><span class="sxs-lookup"><span data-stu-id="c3366-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="c3366-117">Виберіть пункт **користувачі та групи**</span><span class="sxs-lookup"><span data-stu-id="c3366-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="c3366-p105">Цільової певні політики на кого-то, додати їх до списку **включень** . Щоб переконатися, що людина опускається, є політики, додайте їх до списку **виключити** .</span><span class="sxs-lookup"><span data-stu-id="c3366-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="c3366-120">Читати далі: [як пристрої монітор умовного доступу](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="c3366-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

