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
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706776"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="f21c6-102">Налаштування серверів доменних імен для роботи з Microsoft</span><span class="sxs-lookup"><span data-stu-id="f21c6-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="f21c6-103">Примітка. Розповсюдження змін серверів імен може тривати до 48 годин.</span><span class="sxs-lookup"><span data-stu-id="f21c6-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="f21c6-104">Щоб налаштувати домен в Microsoft 365, потрібно оновити сервери імен на сайті реєстратора.</span><span class="sxs-lookup"><span data-stu-id="f21c6-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="f21c6-105">Створіть або змініть записи серверів імен у свого реєстратора доменів.</span><span class="sxs-lookup"><span data-stu-id="f21c6-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="f21c6-106">Перейдіть на веб-сайт реєстратора доменів і знайдіть область, де можна змінити сервери імен.</span><span class="sxs-lookup"><span data-stu-id="f21c6-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="f21c6-107">Створіть або змініть два записи серверів імен із такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="f21c6-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="f21c6-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f21c6-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="f21c6-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="f21c6-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="f21c6-110">Збережіть зміни.</span><span class="sxs-lookup"><span data-stu-id="f21c6-110">Save changes.</span></span>

<span data-ttu-id="f21c6-111">Докладні вказівки наведено в статті [Змінення серверів імен, якщо використовується будь-який реєстратор доменів](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="f21c6-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  