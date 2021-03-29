---
title: Робочий цикл не запускається
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403764"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="c26e0-102">Робочий цикл не запускається</span><span class="sxs-lookup"><span data-stu-id="c26e0-102">Workflow is not starting</span></span>

- <span data-ttu-id="c26e0-103">Робочі цикли SharePoint 2010 і SharePoint 2013 не запускаються.</span><span class="sxs-lookup"><span data-stu-id="c26e0-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="c26e0-104">Якщо робочий цикл не запускається, можуть виникати тимчасові проблеми зі службою, у яких користувачі можуть час відкладати затримки перебігу робочого циклу.</span><span class="sxs-lookup"><span data-stu-id="c26e0-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="c26e0-105">Перегляньте [приладну дошку справності](https://admin.microsoft.com/AdminPortal/Home/servicehealth) служб, щоб дізнатися, чи це впливає на вашу організацію.</span><span class="sxs-lookup"><span data-stu-id="c26e0-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="c26e0-106">Якщо з моменту виникнення цієї проблеми минає понад 24 години, надішлюйте запит на підтримку.</span><span class="sxs-lookup"><span data-stu-id="c26e0-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="c26e0-107">У багатьох випадках ми вже працюємо над вирішенням.</span><span class="sxs-lookup"><span data-stu-id="c26e0-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="c26e0-108">Дайте нам принаймні 24 години, щоб завершити вирішення.</span><span class="sxs-lookup"><span data-stu-id="c26e0-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="c26e0-109">Робочі цикли SharePoint 2010, які затримуються під час запуску.</span><span class="sxs-lookup"><span data-stu-id="c26e0-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="c26e0-110">Це трапляється, якщо робочий цикл запускається великими пакетами.</span><span class="sxs-lookup"><span data-stu-id="c26e0-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="c26e0-111">(Наприклад, якщо одночасно додається кілька елементів).</span><span class="sxs-lookup"><span data-stu-id="c26e0-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="c26e0-112">Робочі цикли не запускаються в реальному часі, тому затримка передбачає певну поведінку.</span><span class="sxs-lookup"><span data-stu-id="c26e0-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="c26e0-113">Якщо робочий цикл – це складна мова розмітки об'єкта (XMOL), компіляція може сповільнюватися.</span><span class="sxs-lookup"><span data-stu-id="c26e0-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="c26e0-114">Перегляньте [цю](https://support.microsoft.com//kb/3043697) статтю.</span><span class="sxs-lookup"><span data-stu-id="c26e0-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="c26e0-115">Слід спростити робочий цикл або перепростити його за допомогою типу платформи робочого циклу Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="c26e0-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="c26e0-116">Якщо журнал робочого циклу збільшується, можливо, ви захочете видалити елементи або створити новий список журналу.</span><span class="sxs-lookup"><span data-stu-id="c26e0-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="c26e0-117">Докладні відомості: [Видалити журнал робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="c26e0-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="c26e0-118">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="c26e0-118">Related topics</span></span>
<span data-ttu-id="c26e0-119">Хочете спробувати Microsoft Flow у SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="c26e0-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="c26e0-120">Створити потік</span><span class="sxs-lookup"><span data-stu-id="c26e0-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c26e0-121">SharePoint і Flow</span><span class="sxs-lookup"><span data-stu-id="c26e0-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
