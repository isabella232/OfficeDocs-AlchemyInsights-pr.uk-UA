---
title: Оновіть сервери імен доменів, щоб вказувати на Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720014"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="148fc-102">Оновіть сервери імен доменів, щоб вказувати на Microsoft</span><span class="sxs-lookup"><span data-stu-id="148fc-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="148fc-103">Примітка. Розповсюдження змін серверів імен може тривати до 48 годин.</span><span class="sxs-lookup"><span data-stu-id="148fc-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="148fc-104">Щоб налаштувати домен з Microsoft, сервери імен у вашому реєстраторі повинні бути оновлені.</span><span class="sxs-lookup"><span data-stu-id="148fc-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="148fc-105">Створіть або змініть записи серверів імен у свого реєстратора доменів.</span><span class="sxs-lookup"><span data-stu-id="148fc-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="148fc-106">Перейдіть на веб-сайт реєстратора доменів і знайдіть область, де можна змінити сервери імен.</span><span class="sxs-lookup"><span data-stu-id="148fc-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="148fc-107">Створіть або змініть два записи серверів імен із такими значеннями:</span><span class="sxs-lookup"><span data-stu-id="148fc-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="148fc-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="148fc-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="148fc-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="148fc-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="148fc-110">Збережіть зміни.</span><span class="sxs-lookup"><span data-stu-id="148fc-110">Save changes.</span></span>

<span data-ttu-id="148fc-111">Ви також можете знайти докладні інструкції в цій статті: [змінити сервери імен для налаштування Microsoft 365 з будь-яким реєстратором домену](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="148fc-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  