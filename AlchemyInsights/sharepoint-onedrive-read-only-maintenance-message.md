---
title: Повідомлення лише для читання, під час спроби використання SharePoint або OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 02cf1aa7abae365a3d317af9e785648d1c1517e1
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051302"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="eda5d-102">Повідомлення лише для читання, під час спроби використання SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="eda5d-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="eda5d-103">Користувачі можуть отримувати повідомлення, **лише для читання** , під час спроби використовувати SharePoint або OneDrive, для одного з таких сценаріїв.</span><span class="sxs-lookup"><span data-stu-id="eda5d-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="eda5d-104">Заплановані або активні обслуговування.</span><span class="sxs-lookup"><span data-stu-id="eda5d-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="eda5d-105">Перевірте їх, перейшовши до [центру повідомлень](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="eda5d-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="eda5d-106">Високий пріоритет, активний інцидент служби, який може трапитися.</span><span class="sxs-lookup"><span data-stu-id="eda5d-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="eda5d-107">Перевірте наявність будь-яких рекомендації/інцидентів, перейшовши до [служби охорони здоров'я](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="eda5d-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="eda5d-108">Неповнолітній Auto-зцілення сценарій відновлення, який може відбуватися через будь-які несподівані події на серверах, які можуть тривати менше 30 хв або близько того.</span><span class="sxs-lookup"><span data-stu-id="eda5d-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="eda5d-109">Є немає повідомлення центру або служби охорони здоров'я посад для цих незначних відновлень, але ви повинні повернутися до нормального найближчим часом.</span><span class="sxs-lookup"><span data-stu-id="eda5d-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="eda5d-110">У дуже небагатьох випадках ми спостерігали, що один з трьох сценаріїв, перерахованих вище, були причиною, і служба була відновлена, але користувачі кеш браузера не був очищений.</span><span class="sxs-lookup"><span data-stu-id="eda5d-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="eda5d-111">Перш ніж перейти на сайт, спробуйте очистити кеш браузера.</span><span class="sxs-lookup"><span data-stu-id="eda5d-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="eda5d-112">У браузері Microsoft EDGE виберіть **настройки**, а потім виберіть **конфіденційність і безпека**.</span><span class="sxs-lookup"><span data-stu-id="eda5d-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="eda5d-113">У розділі **Очистити перегляд**виберіть елемент **вибрати, що слід очистити**.</span><span class="sxs-lookup"><span data-stu-id="eda5d-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="eda5d-114">Виберіть **файли cookie та збережені дані веб-сайтів**, а потім виберіть **Очистити**.</span><span class="sxs-lookup"><span data-stu-id="eda5d-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="eda5d-115">Ці дії можуть відрізнятися під час використання інших браузерів, таких як Mozilla Firefox або Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="eda5d-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="eda5d-116">Іншим варіантом було б відкрити ваш сайт SharePoint або OneDrive у новому вікні InPrivate.</span><span class="sxs-lookup"><span data-stu-id="eda5d-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>