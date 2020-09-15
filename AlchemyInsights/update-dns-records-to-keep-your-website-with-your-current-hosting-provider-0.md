---
title: Оновлення записів DNS для збереження веб-сайту за допомогою поточного постачальника послуг розміщення
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699540"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="d1d57-102">Оновлення записів DNS для збереження веб-сайту за допомогою поточного постачальника послуг розміщення</span><span class="sxs-lookup"><span data-stu-id="d1d57-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="d1d57-103">У центрі адміністрування Microsoft 365 перейдіть на сторінку **настройки**  >  [доменів](https://portal.office.com/adminportal/home#/Domains) , а потім у списку доменів виберіть домен, який використовується для вашого веб-сайту.</span><span class="sxs-lookup"><span data-stu-id="d1d57-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="d1d57-104">Виберіть **+ новий настроюваний запис** і вкажіть такі дії:</span><span class="sxs-lookup"><span data-stu-id="d1d57-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="d1d57-105">У полі **тип DNS** введіть: **A (адреса)**</span><span class="sxs-lookup"><span data-stu-id="d1d57-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="d1d57-106">У полі **ім'я хоста або псевдонім**введіть такі дії: **@**</span><span class="sxs-lookup"><span data-stu-id="d1d57-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="d1d57-107">Для **IP-адреси**введіть СТАТИЧНУ IP-адресу веб-сайту, де він розміщено зараз (наприклад, 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="d1d57-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="d1d57-108">Це має бути  *статична*  IP-адреса веб-сайту, а не  *динамічної*  IP-адреси.</span><span class="sxs-lookup"><span data-stu-id="d1d57-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="d1d57-109">Перевірте сайт, на якому розміщено веб-сайт, щоб переконатися, що ви можете отримати статичну IP-адресу для загальнодоступного веб-сайту.</span><span class="sxs-lookup"><span data-stu-id="d1d57-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="d1d57-110">Натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="d1d57-110">Select **Save**.</span></span>

<span data-ttu-id="d1d57-111">Крім того, можна створити запис CNAME, щоб допомогти користувачам знаходити веб-сайт.</span><span class="sxs-lookup"><span data-stu-id="d1d57-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="d1d57-112">Виберіть **+ новий настроюваний запис** і вкажіть такі дії:</span><span class="sxs-lookup"><span data-stu-id="d1d57-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="d1d57-113">Введіть **тип DNS** : **CNAME (псевдонім)**</span><span class="sxs-lookup"><span data-stu-id="d1d57-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="d1d57-114">У полі **ім'я хоста або псевдонім**введіть таке: **www** .</span><span class="sxs-lookup"><span data-stu-id="d1d57-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="d1d57-115">Для **указує на адресу**введіть повне доменне ім'я (FQDN) для вашого веб-сайту (наприклад, contoso.com).</span><span class="sxs-lookup"><span data-stu-id="d1d57-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="d1d57-116">Натисніть кнопку **зберегти**.</span><span class="sxs-lookup"><span data-stu-id="d1d57-116">Select **Save**.</span></span>
