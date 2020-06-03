---
title: Змінення серверів доменних імен
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: f295e0d7872a13cf47e386343b159e51bc0504de
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508109"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="7c54d-102">Налаштування серверів доменних імен для роботи з Microsoft</span><span class="sxs-lookup"><span data-stu-id="7c54d-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="7c54d-103">Примітка. Розповсюдження змін серверів імен може тривати до 48 годин.</span><span class="sxs-lookup"><span data-stu-id="7c54d-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="7c54d-104">Щоб налаштувати домен в Microsoft 365, потрібно оновити сервери імен на сайті реєстратора.</span><span class="sxs-lookup"><span data-stu-id="7c54d-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="7c54d-105">Створіть або змініть записи серверів імен у свого реєстратора доменів.</span><span class="sxs-lookup"><span data-stu-id="7c54d-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="7c54d-106">Перейдіть на веб-сайт реєстратора доменів і знайдіть область, де можна змінити сервери імен.</span><span class="sxs-lookup"><span data-stu-id="7c54d-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="7c54d-107">Створіть або змініть два записи серверів імен із такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="7c54d-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="7c54d-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7c54d-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="7c54d-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7c54d-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="7c54d-110">Збережіть зміни.</span><span class="sxs-lookup"><span data-stu-id="7c54d-110">Save changes.</span></span>

<span data-ttu-id="7c54d-111">Докладні вказівки наведено в статті [Змінення серверів імен, якщо використовується будь-який реєстратор доменів](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="7c54d-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  