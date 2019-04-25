---
title: Умовного доступу з Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393562"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="19647-102">Умовного доступу з Intune</span><span class="sxs-lookup"><span data-stu-id="19647-102">Conditional Access with Intune</span></span>

<span data-ttu-id="19647-103">За допомогою **Умовного доступу** з Intune вимагає 3 кроки:</span><span class="sxs-lookup"><span data-stu-id="19647-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="19647-104">Створити **Умовного доступу політику** , яка визначає, які ресурси захищений, і те, що умови повинні бути виконані для доступу до цих ресурсів.</span><span class="sxs-lookup"><span data-stu-id="19647-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="19647-105">Наприклад, пристрій має бути сумісний перед отриманням доступу до корпоративної електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="19647-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="19647-106">Створювати **Політику механізми** для визначення параметрів, які повинні бути виконані до пристрою вважається сумісний.</span><span class="sxs-lookup"><span data-stu-id="19647-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="19647-107">Наприклад, пристрій має бути щонайменше 6 цифр PIN-коду до того вважається сумісний.</span><span class="sxs-lookup"><span data-stu-id="19647-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="19647-108">Забезпечення **Дотримання політики** і **Політики умовного доступу** орієнтовані на бажаний груп користувачів.</span><span class="sxs-lookup"><span data-stu-id="19647-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="19647-109">Це може зажадати, створюючи певними групами користувачів у Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="19647-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="19647-110">Читати далі:</span><span class="sxs-lookup"><span data-stu-id="19647-110">Read more:</span></span>
  
- [<span data-ttu-id="19647-111">Умовного доступу кращі практики</span><span class="sxs-lookup"><span data-stu-id="19647-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="19647-112">Початок роботи з умовного доступу</span><span class="sxs-lookup"><span data-stu-id="19647-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

