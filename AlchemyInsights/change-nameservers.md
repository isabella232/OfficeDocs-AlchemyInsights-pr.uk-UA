---
title: Змінення серверів доменних імен
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736670"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="7f27b-102">Налаштування серверів доменних імен для роботи з Office 365</span><span class="sxs-lookup"><span data-stu-id="7f27b-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="7f27b-103">Примітка. Розповсюдження змін серверів імен може тривати до 48 годин.</span><span class="sxs-lookup"><span data-stu-id="7f27b-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="7f27b-104">Щоб налаштувати домен в Office 365, потрібно оновити сервери імен на сайті реєстратора.</span><span class="sxs-lookup"><span data-stu-id="7f27b-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="7f27b-105">Створіть або змініть записи серверів імен у свого реєстратора доменів.</span><span class="sxs-lookup"><span data-stu-id="7f27b-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="7f27b-106">Перейдіть на веб-сайт реєстратора доменів і знайдіть область, де можна змінити сервери імен.</span><span class="sxs-lookup"><span data-stu-id="7f27b-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="7f27b-107">Створіть або змініть два записи серверів імен із такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="7f27b-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="7f27b-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7f27b-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="7f27b-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7f27b-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="7f27b-110">Збережіть зміни.</span><span class="sxs-lookup"><span data-stu-id="7f27b-110">Save changes.</span></span>

<span data-ttu-id="7f27b-111">Докладні вказівки наведено в статті [Змінення DNS-серверів для налаштування Office 365, якщо використовується будь-який реєстратор доменів](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="7f27b-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  