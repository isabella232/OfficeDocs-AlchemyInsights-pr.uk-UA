---
title: Оновлення записів DNS тримати ваш сайт з вашого поточного хостинг-провайдера
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665781"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="f36a3-102">Оновлення записів DNS тримати ваш сайт з вашого поточного хостинг-провайдера</span><span class="sxs-lookup"><span data-stu-id="f36a3-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="f36a3-103">У Microsoft Outlook 365 Центр адміністрування, перейти до **установки** > [домени](https://portal.office.com/adminportal/home#/Domains) сторінку і у списку доменів, виберіть домен, який ви використовуєте для вашого сайту.</span><span class="sxs-lookup"><span data-stu-id="f36a3-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="f36a3-104">Виберіть **+ новий запис користувача** і введіть наступне:</span><span class="sxs-lookup"><span data-stu-id="f36a3-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="f36a3-105">**Тип DNS** введіть: **(адреса)**</span><span class="sxs-lookup"><span data-stu-id="f36a3-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="f36a3-106">Для **імені хоста або псевдонім**введіть таке:**@**</span><span class="sxs-lookup"><span data-stu-id="f36a3-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="f36a3-107">**IP-адреса**введіть статичну ІР-адресу вашого сайту, де вона розташовується в даний час (наприклад, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="f36a3-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="f36a3-108">Це має бути *статична* IP-адреса для сайту, не *динамічний* IP адреса.</span><span class="sxs-lookup"><span data-stu-id="f36a3-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="f36a3-109">Зв'яжіться з сайту, де ваш сайт є розміщення, щоб переконатися, що ви можете отримати статичної IP-адреси для спільних веб-сайтів.</span><span class="sxs-lookup"><span data-stu-id="f36a3-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="f36a3-110">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="f36a3-110">Select **Save**.</span></span>

<span data-ttu-id="f36a3-111">Крім того, ви можете створити запис CNAME, щоб допомогти клієнтам знайти ваш сайт.</span><span class="sxs-lookup"><span data-stu-id="f36a3-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="f36a3-112">Виберіть **+ новий запис користувача** і введіть наступне:</span><span class="sxs-lookup"><span data-stu-id="f36a3-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="f36a3-113">**Тип DNS** введіть: **CNAME (псевдонім)**</span><span class="sxs-lookup"><span data-stu-id="f36a3-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="f36a3-114">**Ім'я хоста або псевдонім**, введіть наступне: **www**</span><span class="sxs-lookup"><span data-stu-id="f36a3-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="f36a3-115">**Вказує на адресу**введіть повне доменне ім'я (FQDN) для вашого веб-сайту (наприклад, "contoso.com").</span><span class="sxs-lookup"><span data-stu-id="f36a3-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="f36a3-116">Виберіть **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="f36a3-116">Select **Save**.</span></span>
