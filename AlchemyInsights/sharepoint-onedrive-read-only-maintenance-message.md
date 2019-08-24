---
title: Читання для обслуговування повідомлення при спробі використовувати SharePoint або OneDrive
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620744"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="ba370-102">Читання для обслуговування повідомлення при спробі використовувати SharePoint або OneDrive</span><span class="sxs-lookup"><span data-stu-id="ba370-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="ba370-103">Користувачі можуть отримувати **Читання для обслуговування** повідомлення при спробі використовувати SharePoint або OneDrive для одного з таких сценаріїв.</span><span class="sxs-lookup"><span data-stu-id="ba370-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="ba370-104">Заплановані або активних технічне обслуговування діяльності.</span><span class="sxs-lookup"><span data-stu-id="ba370-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="ba370-105">Перевірте їх, навігації в [Центрі повідомлень](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="ba370-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="ba370-106">З високим пріоритетом, дійсній службі інцидент, який може бути, що відбуваються.</span><span class="sxs-lookup"><span data-stu-id="ba370-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="ba370-107">Перевірити будь-які рекомендації/інцидентів, перейти на [Службі охорони здоров'я](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ba370-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="ba370-108">Незначні зцілення автоматичного відновлення сценарій, який може відбуватись через будь-які несподівані події на серверах, які можуть тривати протягом менш ніж за 30 хвилин або близько того.</span><span class="sxs-lookup"><span data-stu-id="ba370-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="ba370-109">Там не без повідомлення центр або служби охорони здоров'я повідомлення для цих незначних відшкодувань, але ви повинні бути в норму дуже скоро.</span><span class="sxs-lookup"><span data-stu-id="ba370-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="ba370-110">В дуже небагатьох випадках ми спостерігали, що один з трьох сценаріїв, перерахованих вище були причиною і відновити службу, але кеш браузера користувачі не було з'ясовано.</span><span class="sxs-lookup"><span data-stu-id="ba370-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="ba370-111">Будь ласка намагатися очистити кеш браузера, перш ніж переходити до сайту.</span><span class="sxs-lookup"><span data-stu-id="ba370-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="ba370-112">Браузера Microsoft краю виберіть пункт **настройки**а потім виберіть **конфіденційності та безпеки**.</span><span class="sxs-lookup"><span data-stu-id="ba370-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="ba370-113">У розділі **чітких перегляду**виберіть **Вибрати дані для очищення**.</span><span class="sxs-lookup"><span data-stu-id="ba370-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="ba370-114">Виберіть **файли cookie та дані збережені веб-сайтів**і виберіть **ясно**.</span><span class="sxs-lookup"><span data-stu-id="ba370-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="ba370-115">Ці дії можуть відрізнятися при використанні інших браузерів, таких як Mozilla Firefox або Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="ba370-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="ba370-116">Іншим варіантом було б відкрити сайт SharePoint або OneDrive в новому вікні InPrivate.</span><span class="sxs-lookup"><span data-stu-id="ba370-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>