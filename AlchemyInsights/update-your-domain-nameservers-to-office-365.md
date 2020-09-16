---
title: Налаштування серверів доменних імен для роботи з Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734932"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="7a3a8-102">Налаштування серверів доменних імен для роботи з Microsoft</span><span class="sxs-lookup"><span data-stu-id="7a3a8-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="7a3a8-103">Примітка. Розповсюдження змін серверів імен може тривати до 48 годин.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="7a3a8-104">Щоб настроїти домен корпорацією Майкрософт, DNS-сервери на реєстратора потрібно оновлювати.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="7a3a8-105">Створіть або змініть записи серверів імен у свого реєстратора доменів.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="7a3a8-106">Перейдіть на веб-сайт реєстратора доменів і знайдіть область, де можна змінити сервери імен.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="7a3a8-107">Створіть або змініть два записи серверів імен із такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="7a3a8-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="7a3a8-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7a3a8-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="7a3a8-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7a3a8-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="7a3a8-110">Збережіть зміни.</span><span class="sxs-lookup"><span data-stu-id="7a3a8-110">Save changes.</span></span>

<span data-ttu-id="7a3a8-111">Докладні вказівки можна також знайти в цій статті: [змінення DNS-серверів для настроювання Microsoft 365 за допомогою будь-якого реєстратора доменів](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="7a3a8-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  