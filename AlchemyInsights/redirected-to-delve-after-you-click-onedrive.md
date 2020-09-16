---
title: "\"OneDrive\" для бізнесу веб-OneDrive перенаправляє"
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
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776401"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="5eb49-102">Переспрямовано на "заглиблюватися" після натискання кнопки "OneDrive"</span><span class="sxs-lookup"><span data-stu-id="5eb49-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="5eb49-103">Перегляньте докладні [інструкції з виправлення неполадок](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="5eb49-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="5eb49-104">Щоб вирішити цю проблему, адміністратор повинен надати користувачам право створювати на сайті своїх сайтів.</span><span class="sxs-lookup"><span data-stu-id="5eb49-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="5eb49-105">Це пояснюється тим, що на моїх сайтах створюється сторінка "OneDrive для бізнесу".</span><span class="sxs-lookup"><span data-stu-id="5eb49-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="5eb49-106">Щоб надати це право, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="5eb49-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="5eb49-107">У центрі адміністрування SharePoint виберіть пункт **профілі користувачів**.</span><span class="sxs-lookup"><span data-stu-id="5eb49-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="5eb49-108">У розділі **Контакти** виберіть елемент **Керування дозволами користувача**.</span><span class="sxs-lookup"><span data-stu-id="5eb49-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="5eb49-109">Додайте користувачів, яким потрібні дозволи для створення сайту "мої сайти".</span><span class="sxs-lookup"><span data-stu-id="5eb49-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="5eb49-110">За замовчуванням цей параметр настроєно **всім користувачам, крім зовнішніх користувачів**.</span><span class="sxs-lookup"><span data-stu-id="5eb49-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="5eb49-111">Додавши користувача, користувачів або групу, переконайтеся, що вибрано елемент додано користувача, користувачі або група, прокрутіть до розділу **дозволи** , а потім установіть прапорець **створити персональний сайт (для особистого сховища, каналу новин і переглянутого вмісту)**.</span><span class="sxs-lookup"><span data-stu-id="5eb49-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="5eb49-112">Натисніть кнопку **OK**, а потім користувач має перейти на сторінку OneDrive, щоб створити сайт.</span><span class="sxs-lookup"><span data-stu-id="5eb49-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
