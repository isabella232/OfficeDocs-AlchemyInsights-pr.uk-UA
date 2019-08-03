---
title: Робочий процес не запускається
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171823"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="5a8fa-102">Робочий процес не запускається</span><span class="sxs-lookup"><span data-stu-id="5a8fa-102">Workflow is not starting</span></span>

- <span data-ttu-id="5a8fa-103">SharePoint 2010 і SharePoint 2013 робочі процеси не запускається.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    <span data-ttu-id="5a8fa-104">Якщо робочого процесу не запускається, можливо питання тимчасові обслуговування де користувачів можуть виникнути тимчасовим затримкам з робочого процесу прогресу.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="5a8fa-105">Перевірте [Службу здоров'я Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) щоб побачити, якщо ваша організація є вплив.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    <span data-ttu-id="5a8fa-106">Якщо більш ніж 24 години пройшло з тих пір ви вперше побачив це питання, будь ласка, увійдіть квиток підтримки.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="5a8fa-107">У багатьох випадках ми вже працюємо над вирішенням.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="5a8fa-108">Будь ласка, надайте нам принаймні за 24 години до виконання рішення.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="5a8fa-109">SharePoint 2010 робочі процеси затримується на старті.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-109">SharePoint 2010 workflows delayed on start.</span></span>

    <span data-ttu-id="5a8fa-110">Це відбувається, якщо робочий процес спрацьовує у великих партіях.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="5a8fa-111">(наприклад, коли кілька елементів додаються відразу).</span><span class="sxs-lookup"><span data-stu-id="5a8fa-111">(for example, when several items are added at once).</span></span>

    <span data-ttu-id="5a8fa-112">Робочі процеси не призначений для запуску в режимі реального часу, так що затримка — за дизайн поведінки.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

    <span data-ttu-id="5a8fa-113">Якщо робочий процес комплекс розширюваний об'єктно розмітки мови (XMOL), компіляції може бути повільним.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="5a8fa-114">Перевірити [цю](https://support.microsoft.com/en-us/kb/3043697) статтю.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    <span data-ttu-id="5a8fa-115">Ви повинні спростити робочого процесу або редизайн його за допомогою Microsoft SharePoint робочий процес для 2013 тип платформи.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    <span data-ttu-id="5a8fa-116">Також, якщо робочий процес історії розрісся розмір, ви можете очистити елементи або створити новий список журналу.</span><span class="sxs-lookup"><span data-stu-id="5a8fa-116">Also, if your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

    <span data-ttu-id="5a8fa-117">Більш детальну інформацію: [Очистити історію робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="5a8fa-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="5a8fa-118">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="5a8fa-118">Related topics</span></span>
<span data-ttu-id="5a8fa-119">Хочете спробувати Micrsoft потік в SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="5a8fa-119">Want to try Micrsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="5a8fa-120">Створити потік</span><span class="sxs-lookup"><span data-stu-id="5a8fa-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5a8fa-121">SharePoint і потік</span><span class="sxs-lookup"><span data-stu-id="5a8fa-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


