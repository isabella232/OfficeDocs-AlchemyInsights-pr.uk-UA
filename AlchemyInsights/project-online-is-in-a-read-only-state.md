---
title: Project Online перебуває в стані тільки для читання
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801673"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="f191b-102">Project Online перебуває в стані тільки для читання</span><span class="sxs-lookup"><span data-stu-id="f191b-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="f191b-103">Існує три поширених причин, через які Project Online може досягати стану тільки для читання.</span><span class="sxs-lookup"><span data-stu-id="f191b-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="f191b-104">Організації мають лише ліцензії на веб-сайті Project Online Essentials.</span><span class="sxs-lookup"><span data-stu-id="f191b-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="f191b-105">Це недостатньо для того, щоб зберегти сайт живим, і в кінцевому підсумку вона отримає де-підготовано.</span><span class="sxs-lookup"><span data-stu-id="f191b-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="f191b-106">Ми розміщуємо сайт в стані тільки для читання, щоб адміністратори знали, що щось не так, і можете придбати належні ліцензії.</span><span class="sxs-lookup"><span data-stu-id="f191b-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="f191b-107">Адміністраторам потрібно буде додати ліцензію Project Online Professional і/або Premium.</span><span class="sxs-lookup"><span data-stu-id="f191b-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="f191b-108">Сайт буде виходити лише для читання на цьому етапі.</span><span class="sxs-lookup"><span data-stu-id="f191b-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="f191b-109">Докладні відомості наведено в статті [порівняння рішень з керування проектами](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span><span class="sxs-lookup"><span data-stu-id="f191b-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="f191b-110">Досягнуто квоти.</span><span class="sxs-lookup"><span data-stu-id="f191b-110">Assigned quota has been reached.</span></span> <span data-ttu-id="f191b-111">Щоб отримати докладні відомості, ознайомтеся з [квотою Project Web App](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span><span class="sxs-lookup"><span data-stu-id="f191b-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="f191b-112">Установіть прапорець [настроїти зведення розподілених у часі даних звітування в Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) , щоб дізнатися, як деталізовані звіти можуть вплинути на використання квот.</span><span class="sxs-lookup"><span data-stu-id="f191b-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="f191b-113">Лише для читання може бути дуже тимчасовий стан, який може виникати під час обслуговування.</span><span class="sxs-lookup"><span data-stu-id="f191b-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="f191b-114">Більшість клієнтів навіть не помітили наші клієнти, і ви не побачите цього, але бувають випадки, коли спостерігається короткий період лише для читання.</span><span class="sxs-lookup"><span data-stu-id="f191b-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
