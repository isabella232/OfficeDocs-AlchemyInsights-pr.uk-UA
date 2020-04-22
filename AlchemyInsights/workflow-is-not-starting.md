---
title: Робочий цикл не починається
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 941e6349c98278a1a8cdac77457ec1cc72cdef8b
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766118"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="36744-102">Робочий цикл не починається</span><span class="sxs-lookup"><span data-stu-id="36744-102">Workflow is not starting</span></span>

- <span data-ttu-id="36744-103">SharePoint 2010 і SharePoint 2013 робочі цикли не починаються.</span><span class="sxs-lookup"><span data-stu-id="36744-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="36744-104">Якщо робочий процес не починається, може виникнути проблема тимчасового обслуговування, коли користувачі можуть виникати періодичні затримки з прогресом робочого циклу.</span><span class="sxs-lookup"><span data-stu-id="36744-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="36744-105">Перегляньте [приладну дошку стану служби](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб дізнатися, чи впливає ваша організація.</span><span class="sxs-lookup"><span data-stu-id="36744-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="36744-106">Якщо Минуло більше 24 годин з тих пір, як ви вперше побачили цю проблему, будь ласка, увійдіть квиток підтримки.</span><span class="sxs-lookup"><span data-stu-id="36744-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="36744-107">У багатьох випадках ми вже працюємо над вирішенням.</span><span class="sxs-lookup"><span data-stu-id="36744-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="36744-108">Будь ласка, дайте нам принаймні 24 годин, щоб завершити рішення.</span><span class="sxs-lookup"><span data-stu-id="36744-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="36744-109">SharePoint 2010 робочі цикли, затримуються на початковому запуску.</span><span class="sxs-lookup"><span data-stu-id="36744-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="36744-110">Це відбувається, якщо робочий цикл запускається великими партіями.</span><span class="sxs-lookup"><span data-stu-id="36744-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="36744-111">(наприклад, коли кілька елементів додаються одночасно).</span><span class="sxs-lookup"><span data-stu-id="36744-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="36744-112">Робочі цикли не призначені для запуску в режимі реального часу, тому затримка є за-дизайн поведінки.</span><span class="sxs-lookup"><span data-stu-id="36744-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="36744-113">Якщо робочий процес складний, розширювана об'єкт розмітки мови (XMOL), компіляції може бути повільним.</span><span class="sxs-lookup"><span data-stu-id="36744-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="36744-114">Перевірити [цю](https://support.microsoft.com//kb/3043697) статтю.</span><span class="sxs-lookup"><span data-stu-id="36744-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="36744-115">Ви повинні спростити робочий цикл або переробити його за допомогою типу платформи робочого циклу Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="36744-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="36744-116">Якщо історія робочого циклу зросла, можливо, потрібно видалити елементи або створити новий список журналу.</span><span class="sxs-lookup"><span data-stu-id="36744-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="36744-117">Додаткові відомості: [очищення журналу робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="36744-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="36744-118">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="36744-118">Related topics</span></span>
<span data-ttu-id="36744-119">Бажаєте спробувати Microsoft Flow у SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="36744-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="36744-120">Створити потік</span><span class="sxs-lookup"><span data-stu-id="36744-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="36744-121">SharePoint і Flow</span><span class="sxs-lookup"><span data-stu-id="36744-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


