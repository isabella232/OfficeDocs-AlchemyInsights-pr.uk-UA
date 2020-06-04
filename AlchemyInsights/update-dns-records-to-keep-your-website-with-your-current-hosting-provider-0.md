---
title: Оновлення записів DNS для збереження веб-сайту за допомогою поточного постачальника послуг хостингу
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665781"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="127e0-102">Оновлення записів DNS для збереження веб-сайту за допомогою поточного постачальника послуг хостингу</span><span class="sxs-lookup"><span data-stu-id="127e0-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="127e0-103">У центрі адміністрування Microsoft 365 перейдіть на сторінку **Настроювання**  >  [доменів](https://portal.office.com/adminportal/home#/Domains) і у списку доменів виберіть домен, який ви використовуєте для вашого веб-сайту.</span><span class="sxs-lookup"><span data-stu-id="127e0-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="127e0-104">Виберіть **+ новий користувацький запис** і введіть наступне:</span><span class="sxs-lookup"><span data-stu-id="127e0-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="127e0-105">Для **DNS** введіть: **A (адреса)**</span><span class="sxs-lookup"><span data-stu-id="127e0-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="127e0-106">Для **імені хоста або псевдоніма**введіть таке:**@**</span><span class="sxs-lookup"><span data-stu-id="127e0-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="127e0-107">Для **IP-адреси**введіть статичну ІР-адресу вашого веб-сайту, де він наразі розміщується (наприклад, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="127e0-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="127e0-108">Це має бути *статична* IP-адреса для веб-сайту, а не *динамічна* ІР-адреса.</span><span class="sxs-lookup"><span data-stu-id="127e0-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="127e0-109">Перевірте з сайтом, де розміщений ваш веб-сайт, щоб переконатися, що ви можете отримати статичний IP-адресу для вашого публічного веб-сайту.</span><span class="sxs-lookup"><span data-stu-id="127e0-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="127e0-110">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="127e0-110">Select **Save**.</span></span>

<span data-ttu-id="127e0-111">Крім того, можна створити запис CNAME, щоб допомогти користувачам знайти ваш веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="127e0-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="127e0-112">Виберіть **+ новий користувацький запис** і введіть наступне:</span><span class="sxs-lookup"><span data-stu-id="127e0-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="127e0-113">Для **DNS введіть** : **CNAME (псевдонім)**</span><span class="sxs-lookup"><span data-stu-id="127e0-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="127e0-114">Для **імені хоста або псевдоніма**введіть таке: **www**</span><span class="sxs-lookup"><span data-stu-id="127e0-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="127e0-115">Для **пунктів адреси**введіть повне доменне ім'я (FQDN) для вашого веб-сайту (наприклад, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="127e0-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="127e0-116">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="127e0-116">Select **Save**.</span></span>
