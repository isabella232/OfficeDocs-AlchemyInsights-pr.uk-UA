---
title: Оновлення записів DNS для збереження веб-сайту в поточного постачальника послуг розміщення
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827561"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="506fa-102">Оновлення записів DNS для збереження веб-сайту в поточного постачальника послуг розміщення</span><span class="sxs-lookup"><span data-stu-id="506fa-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="506fa-103">У Центрі адміністрування Microsoft 365 перейдіть на сторінку Настроювання доменів і зі списку доменів виберіть домен, який використовується для  >  [](https://admin.microsoft.com/Adminportal#/Domains) веб-сайту.</span><span class="sxs-lookup"><span data-stu-id="506fa-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="506fa-104">Виберіть **+ Новий спеціальний запис** і введіть такі дані:</span><span class="sxs-lookup"><span data-stu-id="506fa-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="506fa-105">Для **типу DNS введіть** A **(адреса).**</span><span class="sxs-lookup"><span data-stu-id="506fa-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="506fa-106">У **полі Ім'я хоста або Псевдонім** введіть таке: **@**</span><span class="sxs-lookup"><span data-stu-id="506fa-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="506fa-107">У **полі IP-адреса** введіть статичну IP-адресу для поточного веб-сайту (наприклад, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="506fa-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="506fa-108">Це має бути *статична IP-адреса* веб-сайту, а не *динамічна.*</span><span class="sxs-lookup"><span data-stu-id="506fa-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="506fa-109">Зверніться до сайту, на якому розміщено ваш веб-сайт, щоб переконатися, що ви можете отримати статичну IP-адресу для загальнодоступного веб-сайту.</span><span class="sxs-lookup"><span data-stu-id="506fa-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="506fa-110">Натисніть **кнопку Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="506fa-110">Select **Save**.</span></span>

<span data-ttu-id="506fa-111">Крім того, можна створити запис CNAME, який допоможе клієнтам знайти ваш веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="506fa-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="506fa-112">Виберіть **+ Новий спеціальний запис** і введіть такі дані:</span><span class="sxs-lookup"><span data-stu-id="506fa-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="506fa-113">Для **типу DNS введіть** **CNAME (псевдонім)**</span><span class="sxs-lookup"><span data-stu-id="506fa-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="506fa-114">У **полі Ім'я хоста або псевдонім** введіть **www.**</span><span class="sxs-lookup"><span data-stu-id="506fa-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="506fa-115">У **полі Указує** на адресу введіть повне доменне ім'я (FQDN) свого веб-сайту (наприклад, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="506fa-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="506fa-116">Натисніть **кнопку Зберегти**.</span><span class="sxs-lookup"><span data-stu-id="506fa-116">Select **Save**.</span></span>
