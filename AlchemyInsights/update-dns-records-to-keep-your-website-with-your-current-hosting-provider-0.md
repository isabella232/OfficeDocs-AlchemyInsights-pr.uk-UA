---
title: Оновлення записів DNS тримати ваш сайт з вашого поточного хостинг-провайдера
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
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
ms.openlocfilehash: a1ea0589def4945da64c73d68b2e4a3d64d6b83d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506428"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="9e984-102">Оновлення записів DNS тримати ваш сайт з вашого поточного хостинг-провайдера</span><span class="sxs-lookup"><span data-stu-id="9e984-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="9e984-103">На сторінці [домени](https://portal.office.com/adminportal/home#/Domains) » у списку доменів, виберіть домен, який ви використовуєте для вашого сайту.</span><span class="sxs-lookup"><span data-stu-id="9e984-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="9e984-104">Виберіть **+ новий запис користувача** і введіть наступне:</span><span class="sxs-lookup"><span data-stu-id="9e984-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9e984-105">**Тип DNS** введіть: **(адреса)**</span><span class="sxs-lookup"><span data-stu-id="9e984-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="9e984-106">Для **імені хоста або псевдонім**введіть таке:**@**</span><span class="sxs-lookup"><span data-stu-id="9e984-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="9e984-107">**IP-адреса**введіть статичну ІР-адресу вашого сайту, де вона розташовується в даний час (наприклад, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="9e984-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="9e984-108">Це має бути *статична* IP-адреса для сайту, не *динамічний* IP адреса.</span><span class="sxs-lookup"><span data-stu-id="9e984-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="9e984-109">Зв'яжіться з сайту, де ваш сайт є розміщення, щоб переконатися, що ви можете отримати статичної IP-адреси для спільних веб-сайтів.</span><span class="sxs-lookup"><span data-stu-id="9e984-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="9e984-110">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="9e984-110">Select **Save**.</span></span>

<span data-ttu-id="9e984-111">Крім того, ви можете створити запис CNAME, щоб допомогти клієнтам знайти ваш сайт.</span><span class="sxs-lookup"><span data-stu-id="9e984-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="9e984-112">Виберіть **+ новий запис користувача** і введіть наступне:</span><span class="sxs-lookup"><span data-stu-id="9e984-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="9e984-113">**Тип DNS** введіть: **CNAME (псевдонім)**</span><span class="sxs-lookup"><span data-stu-id="9e984-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="9e984-114">**Ім'я хоста або псевдонім**, введіть наступне: **www**</span><span class="sxs-lookup"><span data-stu-id="9e984-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="9e984-115">**Вказує на адресу**введіть повне доменне ім'я (FQDN) для вашого веб-сайту (наприклад, "contoso.com").</span><span class="sxs-lookup"><span data-stu-id="9e984-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="9e984-116">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="9e984-116">Select **Save**.</span></span>
