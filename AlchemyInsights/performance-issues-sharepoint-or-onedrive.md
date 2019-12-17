---
title: Проблеми продуктивності-SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068442"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="2bbe5-102">SharePoint або OneDrive, повільно, недоступний або недоступний для кількох користувачів</span><span class="sxs-lookup"><span data-stu-id="2bbe5-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="2bbe5-103">SharePoint або OneDrive можуть бути повільними, недоступними або недоступні, або може відображатися Служба недоступна або 503 помилки, з кількох причин:</span><span class="sxs-lookup"><span data-stu-id="2bbe5-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="2bbe5-104">Якщо ваш сайт SharePoint або OneDrive уповільнюється або затримується для кількох користувачів, може виникнути проблема тимчасового обслуговування, коли користувачі відчувають періодичні затримки або помилки навігації під час доступу до сайтів SharePoint або вмісту OneDrive.</span><span class="sxs-lookup"><span data-stu-id="2bbe5-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="2bbe5-105">Перегляньте [приладну дошку стану служби](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб дізнатися, чи впливає ваша організація.</span><span class="sxs-lookup"><span data-stu-id="2bbe5-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="2bbe5-106">Користувачі можуть отримувати *503 сервер зайнятий* , помилка під час спроби перейти до SharePoint або OneDrive сайтів.</span><span class="sxs-lookup"><span data-stu-id="2bbe5-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="2bbe5-107">Ця помилка може бути викликана дроселювання у службі SharePoint.</span><span class="sxs-lookup"><span data-stu-id="2bbe5-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="2bbe5-108">SharePoint Online використовує дроселювання для підтримки оптимальної продуктивності та надійності служби SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="2bbe5-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="2bbe5-109">Дроселювання обмежує кількість дій користувача або одночасних викликів (за сценарієм або кодом) для запобігання надмірного використання ресурсів.</span><span class="sxs-lookup"><span data-stu-id="2bbe5-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="2bbe5-110">Для отримання додаткових відомостей про дроселювання можна [уникнути обмеження або блокування в SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="2bbe5-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="2bbe5-111">Якщо спостерігається низька швидкодія за допомогою **класичного** або **сучасного** сайту SharePoint або сторінки, використовуйте [засіб діагностики сторінок](https://aka.ms/perftool) для аналізу сторінок.</span><span class="sxs-lookup"><span data-stu-id="2bbe5-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="2bbe5-112">Якщо ви все ще відчуваєте загальне зниження продуктивності, будь ласка, перегляньте ресурси в нижній частині цієї статті: [вступ до налаштування продуктивності для SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="2bbe5-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  