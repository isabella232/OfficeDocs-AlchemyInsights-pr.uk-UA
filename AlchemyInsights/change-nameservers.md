---
title: Змінення серверів доменних імен
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818633"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="fd7b3-102">Налаштування серверів доменних імен для роботи з Microsoft</span><span class="sxs-lookup"><span data-stu-id="fd7b3-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="fd7b3-103">Примітка. Розповсюдження змін серверів імен може тривати до 48 годин.</span><span class="sxs-lookup"><span data-stu-id="fd7b3-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="fd7b3-104">Щоб налаштувати домен в Microsoft 365, потрібно оновити сервери імен на сайті реєстратора.</span><span class="sxs-lookup"><span data-stu-id="fd7b3-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="fd7b3-105">Створіть або змініть записи серверів імен у свого реєстратора доменів.</span><span class="sxs-lookup"><span data-stu-id="fd7b3-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="fd7b3-106">Перейдіть на веб-сайт реєстратора доменів і знайдіть область, де можна змінити сервери імен.</span><span class="sxs-lookup"><span data-stu-id="fd7b3-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="fd7b3-107">Створіть або змініть два записи серверів імен із такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="fd7b3-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="fd7b3-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="fd7b3-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="fd7b3-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="fd7b3-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="fd7b3-110">Збережіть зміни.</span><span class="sxs-lookup"><span data-stu-id="fd7b3-110">Save changes.</span></span>

<span data-ttu-id="fd7b3-111">Докладні вказівки наведено в статті [Змінення серверів імен, якщо використовується будь-який реєстратор доменів](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="fd7b3-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  