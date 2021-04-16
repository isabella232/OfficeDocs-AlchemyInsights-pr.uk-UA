---
title: Переспрямування OneDrive для бізнесу до Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51800010"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="abdf8-102">Переспрямування до Delve після натискання кнопки OneDrive</span><span class="sxs-lookup"><span data-stu-id="abdf8-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="abdf8-103">Перегляньте наш [докладний посібник із виправлення неполадок.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="abdf8-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="abdf8-104">Щоб вирішити цю проблему, адміністратор повинен надати користувачам право створювати свої сайти "Мій сайт".</span><span class="sxs-lookup"><span data-stu-id="abdf8-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="abdf8-105">Це зумовлює створення сторінки служби OneDrive для бізнесу на сторінці "Мої сайти".</span><span class="sxs-lookup"><span data-stu-id="abdf8-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="abdf8-106">Щоб надати це право, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="abdf8-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="abdf8-107">У Центрі адміністрування SharePoint клацніть **Профілі користувачів.**</span><span class="sxs-lookup"><span data-stu-id="abdf8-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="abdf8-108">У розділі **Контакти** клацніть елемент Керування **дозволами користувача.**</span><span class="sxs-lookup"><span data-stu-id="abdf8-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="abdf8-109">Додайте користувачів, яким потрібні дозволи на створення сайту "Мій сайт".</span><span class="sxs-lookup"><span data-stu-id="abdf8-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="abdf8-110">За замовчуванням для цього параметра встановлено значення Усі, **крім зовнішніх користувачів.**</span><span class="sxs-lookup"><span data-stu-id="abdf8-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="abdf8-111">Додавши користувача, користувачів або групу, переконайтеся, що встановлено прапорець доданого користувача, користувачів або групи, прокрутіть до розділу дозволів і встановіть прапорець Створити особистий сайт (потрібен для особистого сховища, каналу новин і відслідковуваного **вмісту).** </span><span class="sxs-lookup"><span data-stu-id="abdf8-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="abdf8-112">Натисніть **кнопку OK,** а потім зайдіть на сторінку OneDrive, щоб створити сайт.</span><span class="sxs-lookup"><span data-stu-id="abdf8-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
