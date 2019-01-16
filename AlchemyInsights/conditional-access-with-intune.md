---
title: Умовного доступу з Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28318796"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="19637-102">Умовного доступу з Intune</span><span class="sxs-lookup"><span data-stu-id="19637-102">Conditional Access with Intune</span></span>

<span data-ttu-id="19637-103">За допомогою **Умовного доступу** з Intune вимагає 3 кроки:</span><span class="sxs-lookup"><span data-stu-id="19637-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="19637-p101">Створити **Умовного доступу політику** , яка визначає, які ресурси захищений, і те, що умови повинні бути виконані для доступу до цих ресурсів. Наприклад, пристрій має бути сумісний перед отриманням доступу до корпоративної електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="19637-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="19637-p102">Створювати **Політику механізми** для визначення параметрів, які повинні бути виконані до пристрою вважається сумісний. Наприклад, пристрій має бути щонайменше 6 цифр PIN-коду до того вважається сумісний.</span><span class="sxs-lookup"><span data-stu-id="19637-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="19637-p103">Забезпечення **Дотримання політики** і **Політики умовного доступу** орієнтовані на бажаний груп користувачів. Це може зажадати, створюючи певними групами користувачів у Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="19637-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="19637-110">Читати далі:</span><span class="sxs-lookup"><span data-stu-id="19637-110">Read more:</span></span>
  
- [<span data-ttu-id="19637-111">Умовного доступу кращі практики</span><span class="sxs-lookup"><span data-stu-id="19637-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="19637-112">Початок роботи з умовного доступу</span><span class="sxs-lookup"><span data-stu-id="19637-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

