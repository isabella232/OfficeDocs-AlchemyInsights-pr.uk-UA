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
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505015"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="616ab-102">Умовного доступу з Intune</span><span class="sxs-lookup"><span data-stu-id="616ab-102">Conditional Access with Intune</span></span>

<span data-ttu-id="616ab-103">За допомогою **Умовного доступу** з Intune вимагає 3 кроки:</span><span class="sxs-lookup"><span data-stu-id="616ab-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="616ab-104">Створити **Умовного доступу політику** , яка визначає, які ресурси захищений, і те, що умови повинні бути виконані для доступу до цих ресурсів.</span><span class="sxs-lookup"><span data-stu-id="616ab-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="616ab-105">Наприклад, пристрій має бути сумісний перед отриманням доступу до корпоративної електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="616ab-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="616ab-106">Створювати **Політику механізми** для визначення параметрів, які повинні бути виконані до пристрою вважається сумісний.</span><span class="sxs-lookup"><span data-stu-id="616ab-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="616ab-107">Наприклад, пристрій має бути щонайменше 6 цифр PIN-коду до того вважається сумісний.</span><span class="sxs-lookup"><span data-stu-id="616ab-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="616ab-108">Забезпечення **Дотримання політики** і **Політики умовного доступу** орієнтовані на бажаний груп користувачів.</span><span class="sxs-lookup"><span data-stu-id="616ab-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="616ab-109">Це може зажадати, створюючи певними групами користувачів у Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="616ab-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="616ab-110">Читати далі:</span><span class="sxs-lookup"><span data-stu-id="616ab-110">Read more:</span></span>
  
- [<span data-ttu-id="616ab-111">Умовного доступу кращі практики</span><span class="sxs-lookup"><span data-stu-id="616ab-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="616ab-112">Початок роботи з умовного доступу</span><span class="sxs-lookup"><span data-stu-id="616ab-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

