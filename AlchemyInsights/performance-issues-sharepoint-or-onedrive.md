---
title: Проблеми з продуктивністю – SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771922"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="29b10-102">Служба SharePoint або OneDrive низька, недоступна або недоступна для кількох користувачів</span><span class="sxs-lookup"><span data-stu-id="29b10-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="29b10-103">Служба SharePoint або OneDrive може бути повільною, недосяжно або недоступна або може відображати служби, недоступні або 503 помилки, з кількох причин.</span><span class="sxs-lookup"><span data-stu-id="29b10-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="29b10-104">Якщо на сайті SharePoint або OneDrive повільне або відкладено для кількох користувачів, може виникнути тимчасова проблема служби, у якій користувачі можуть періодично затримуватися або під час переходу під час доступу до сайтів SharePoint або вмісту OneDrive.</span><span class="sxs-lookup"><span data-stu-id="29b10-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="29b10-105">Перевірте [приладну дошку справності служби](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб дізнатися, чи впливає ваша організація.</span><span class="sxs-lookup"><span data-stu-id="29b10-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="29b10-106">Користувачі можуть отримувати повідомлення про помилку *сервера 503* під час спроби переходу на сайти SharePoint або OneDrive.</span><span class="sxs-lookup"><span data-stu-id="29b10-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="29b10-107">Ця помилка може бути спричинена дроселювання в межах служби SharePoint.</span><span class="sxs-lookup"><span data-stu-id="29b10-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="29b10-108">Служба SharePoint Online використовує дроселювання, щоб забезпечити оптимальну продуктивність і надійність.</span><span class="sxs-lookup"><span data-stu-id="29b10-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="29b10-109">Дроселювання обмежує кількість дій користувачів або одночасних викликів (за сценарієм або кодом), щоб уникнути надмірного використання ресурсів.</span><span class="sxs-lookup"><span data-stu-id="29b10-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="29b10-110">Щоб отримати докладніші відомості про дроселювання, Дізнайтеся, [як уникнути обмеження або блокування в службі SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="29b10-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="29b10-111">Якщо ви зменшите продуктивність за допомогою **класичного** або **сучасного** сайту SharePoint або сторінки, скористайтеся [засобом діагностики сторінки](https://aka.ms/perftool) , щоб аналізувати сторінки.</span><span class="sxs-lookup"><span data-stu-id="29b10-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="29b10-112">Якщо ви ще не змогли виконати загальну повільну продуктивність, перегляньте ресурси в нижній частині цієї статті: [Загальні відомості про настроювання продуктивності для служби SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="29b10-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  