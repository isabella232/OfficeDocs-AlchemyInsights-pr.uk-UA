---
title: Моніторинг умовного доступу
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538801"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="62b20-102">Моніторинг умовного доступу для обміну</span><span class="sxs-lookup"><span data-stu-id="62b20-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="62b20-103">Користувачі націлено на умовного доступу будуть отримувати повідомлення по електронній пошті, якщо вони не відповідають вимогам доступ до вашої організації.</span><span class="sxs-lookup"><span data-stu-id="62b20-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="62b20-104">Щоб вирішити, ми рекомендуємо одну або кілька з таких рішень:</span><span class="sxs-lookup"><span data-stu-id="62b20-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="62b20-105">Якщо пристрій, як припускають, повинен бути, повідомити користувача зайти на портал компанії app і переконайтеся, що він з'являється на порталі компанії.</span><span class="sxs-lookup"><span data-stu-id="62b20-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="62b20-106">Якщо цього не відбувається, користувач повинен зареєструвати пристрою.</span><span class="sxs-lookup"><span data-stu-id="62b20-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="62b20-107">Блакитні на порталі перейдіть на **Intune \> пристрій дотримання**.</span><span class="sxs-lookup"><span data-stu-id="62b20-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="62b20-108">У розділі **монітор** натисніть **пристрій відповідності**.</span><span class="sxs-lookup"><span data-stu-id="62b20-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="62b20-109">Переглянути ваш пристрій дотримання звіту для перевірки пристрою користувача буде позначено як сумісні.</span><span class="sxs-lookup"><span data-stu-id="62b20-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="62b20-110">Блакитні на порталі перейдіть на **Intune \> пристрій дотримання**.</span><span class="sxs-lookup"><span data-stu-id="62b20-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="62b20-111">У розділі **керування**клацніть **політику**.</span><span class="sxs-lookup"><span data-stu-id="62b20-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="62b20-112">У списку дотримання політики перевірте, чи профіль призначається для вашого користувача пристрою.</span><span class="sxs-lookup"><span data-stu-id="62b20-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="62b20-113">Якщо немає профілю присвоюється, потім Intune не буде може підтвердити відповідність стану пристрою.</span><span class="sxs-lookup"><span data-stu-id="62b20-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="62b20-114">Редагування поступки умовного доступу користувача.</span><span class="sxs-lookup"><span data-stu-id="62b20-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="62b20-115">Блакитні на порталі перейдіть на **Intune \> умовного доступу \> політики**</span><span class="sxs-lookup"><span data-stu-id="62b20-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="62b20-116">Виберіть політику зі списку</span><span class="sxs-lookup"><span data-stu-id="62b20-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="62b20-117">Виберіть пункт **користувачі та групи**</span><span class="sxs-lookup"><span data-stu-id="62b20-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="62b20-118">Цільової певні політики на кого-то, додати їх до списку **включень** .</span><span class="sxs-lookup"><span data-stu-id="62b20-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="62b20-119">Щоб переконатися, що людина опускається, є політики, додайте їх до списку **виключити** .</span><span class="sxs-lookup"><span data-stu-id="62b20-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="62b20-120">Читати далі: [як пристрої монітор умовного доступу](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="62b20-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

