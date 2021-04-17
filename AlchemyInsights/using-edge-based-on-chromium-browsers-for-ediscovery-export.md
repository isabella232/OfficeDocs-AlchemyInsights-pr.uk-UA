---
title: Використання Microsoft Edge на основі браузерів Chromium для експорту Ediscovery
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834392"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="91acf-102">Використання Microsoft Edge на основі браузерів Chromium для експорту Ediscovery</span><span class="sxs-lookup"><span data-stu-id="91acf-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="91acf-103">Через нещодавню зміну браузери Microsoft Edge більше не зможуть підтримувати ClickOnce за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="91acf-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="91acf-104">Щоб і надалі використовувати засіб експорту витребування електронної пошти Microsoft 365, потрібно скористатися браузером Microsoft Internet Explorer або ввімкнути підтримку ClickOnce у Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="91acf-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="91acf-105">Щоб увімкнути підтримку ClickOnce у Microsoft Edge на основі Chromium:</span><span class="sxs-lookup"><span data-stu-id="91acf-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="91acf-106">У браузері Microsoft Edge відвідайте веб edge://flags/#edge-click-once.</span><span class="sxs-lookup"><span data-stu-id="91acf-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="91acf-107">Для параметра Підтримка ClickOnce змініть значення з значення За замовчуванням або Вимкнуто **на**  Увімкнуто. </span><span class="sxs-lookup"><span data-stu-id="91acf-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="91acf-108">У нижній частині вікна браузера натисніть кнопку **Перезавантажити**.</span><span class="sxs-lookup"><span data-stu-id="91acf-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="91acf-109">Зміни наберуть сили після перезапуску Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="91acf-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="91acf-110">Відомості про це та інструкції з інсталяції засобу експорту див. в статті [Експорт результатів пошуку вмісту.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="91acf-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>