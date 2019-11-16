---
title: Умовний доступ з InTune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36505015"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="131a5-102">Умовний доступ з InTune</span><span class="sxs-lookup"><span data-stu-id="131a5-102">Conditional Access with Intune</span></span>

<span data-ttu-id="131a5-103">За допомогою **умовного доступу** з InTune потрібно 3 кроки:</span><span class="sxs-lookup"><span data-stu-id="131a5-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="131a5-104">Створіть **політику умовного доступу** , яка визначає, які ресурси захищено, і які умови повинні бути виконані для доступу до цих ресурсів.</span><span class="sxs-lookup"><span data-stu-id="131a5-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="131a5-105">Наприклад, пристрій має відповідати вимогам, перш ніж отримати доступ до корпоративної електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="131a5-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="131a5-106">Створіть **політику відповідності** , щоб визначити параметри, які повинні бути виконані перед тим, як пристрій вважається сумісним.</span><span class="sxs-lookup"><span data-stu-id="131a5-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="131a5-107">Наприклад, пристрій повинен мати PIN-код принаймні 6 цифр, перш ніж він вважатиметься сумісним.</span><span class="sxs-lookup"><span data-stu-id="131a5-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="131a5-108">Забезпечення як **політики відповідності** , так і **політики умовного доступу** орієнтовані на потрібних груп користувачів.</span><span class="sxs-lookup"><span data-stu-id="131a5-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="131a5-109">Це може знадобитися, створення певних груп користувачів у Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="131a5-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="131a5-110">Читати далі:</span><span class="sxs-lookup"><span data-stu-id="131a5-110">Read more:</span></span>
  
- [<span data-ttu-id="131a5-111">Практичні поради щодо умовного доступу</span><span class="sxs-lookup"><span data-stu-id="131a5-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="131a5-112">Початок роботи з умовним доступом</span><span class="sxs-lookup"><span data-stu-id="131a5-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

