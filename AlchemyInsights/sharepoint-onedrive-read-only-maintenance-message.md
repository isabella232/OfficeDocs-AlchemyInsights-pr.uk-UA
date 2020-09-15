---
title: Під час спроби використовувати службу SharePoint або OneDrive можна тільки для читання.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670853"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="4c1a1-102">Під час спроби використовувати службу SharePoint або OneDrive можна тільки для читання.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="4c1a1-103">Користувачі можуть отримувати повідомлення **лише для читання** , коли ви намагаєтеся використовувати SharePoint або OneDrive для одного з наведених нижче сценаріїв.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="4c1a1-104">Заплановані або активні дії з обслуговування.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="4c1a1-105">Перевірте їх, перейшовши до [центру повідомлень](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="4c1a1-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="4c1a1-106">Високий пріоритет, активна служба, що може бути відбувається.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="4c1a1-107">Перегляньте всі рекомендації та інциденти, перейшовши до [справності служби](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4c1a1-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="4c1a1-108">Незначний сценарій відновлення для автоматичного зцілення, який може відбуватися через непередбачені події на серверах, які можуть тривати менше 30 хв.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="4c1a1-109">Для цих незначних відшкодувань немає повідомлень або служб для медичних повідомлень, але ви маєте повернутися до нормального.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="4c1a1-110">У дуже мало випадків ми спостерігали, що один із трьох сценаріїв, перерахованих вище, було причиною, а служба відновлено, але кеш браузера користувачів не очищено.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="4c1a1-111">Перш ніж переходити до сайту, спробуйте очистити кеш браузера.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="4c1a1-112">У браузері Microsoft EDGE натисніть кнопку **настройки**, а потім виберіть пункт **конфіденційність і безпека**.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="4c1a1-113">У розділі **Очистити перегляд**виберіть пункт **вибрати, що потрібно очистити**.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="4c1a1-114">Виберіть **файли cookie та збережені дані веб-сайту**, а потім натисніть кнопку **Очистити**.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="4c1a1-115">Ці дії можуть відрізнятися під час використання інших браузерів, таких як Mozilla Firefox або Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="4c1a1-116">Інший варіант – відкрити сайт SharePoint або OneDrive в новому вікні InPrivate.</span><span class="sxs-lookup"><span data-stu-id="4c1a1-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>