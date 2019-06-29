---
title: Налаштування серверів доменних імен для роботи з Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 8e25c510233f2a00d133ea69a338141c5a475465
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35352910"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="a88a9-102">Налаштування серверів доменних імен для роботи з Office 365</span><span class="sxs-lookup"><span data-stu-id="a88a9-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="a88a9-103">Примітка. Розповсюдження змін серверів імен може тривати до 48 годин.</span><span class="sxs-lookup"><span data-stu-id="a88a9-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="a88a9-104">Щоб налаштувати домен в Office 365, потрібно оновити сервери імен на сайті реєстратора.</span><span class="sxs-lookup"><span data-stu-id="a88a9-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="a88a9-105">Створіть або змініть записи серверів імен у свого реєстратора доменів.</span><span class="sxs-lookup"><span data-stu-id="a88a9-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="a88a9-106">Перейдіть на веб-сайт реєстратора доменів і знайдіть область, де можна змінити сервери імен.</span><span class="sxs-lookup"><span data-stu-id="a88a9-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="a88a9-107">Створіть або змініть два записи серверів імен із такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="a88a9-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="a88a9-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a88a9-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="a88a9-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="a88a9-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="a88a9-110">Збережіть зміни.</span><span class="sxs-lookup"><span data-stu-id="a88a9-110">Save changes.</span></span>

<span data-ttu-id="a88a9-111">Докладні вказівки наведено в статті [Змінення DNS-серверів для налаштування Office 365, якщо використовується будь-який реєстратор доменів](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="a88a9-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  