---
title: Запуск робочого циклу не починається
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794788"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="9973e-102">Запуск робочого циклу не починається</span><span class="sxs-lookup"><span data-stu-id="9973e-102">Workflow is not starting</span></span>

- <span data-ttu-id="9973e-103">Робочі цикли SharePoint 2010 і SharePoint 2013 не починаються.</span><span class="sxs-lookup"><span data-stu-id="9973e-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="9973e-104">Якщо робочий цикл не запускається, може виникнути тимчасова проблема служби, у якій користувачі можуть виникати періодичні затримки з прогресом робочого циклу.</span><span class="sxs-lookup"><span data-stu-id="9973e-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="9973e-105">Перевірте [приладну дошку справності служби](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , щоб дізнатися, чи впливає ваша організація.</span><span class="sxs-lookup"><span data-stu-id="9973e-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="9973e-106">Якщо ви вперше побачили цю проблему понад 24 години, увійдіть у службу підтримки.</span><span class="sxs-lookup"><span data-stu-id="9973e-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9973e-107">У багатьох випадках ми вже працюємо над вирішенням проблеми.</span><span class="sxs-lookup"><span data-stu-id="9973e-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9973e-108">Щоб завершити вирішення, надайте нам принаймні 24 години.</span><span class="sxs-lookup"><span data-stu-id="9973e-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="9973e-109">Робочі цикли SharePoint 2010, затримані під час запуску.</span><span class="sxs-lookup"><span data-stu-id="9973e-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="9973e-110">Це трапляється, якщо робочий цикл запущено у великих партіях.</span><span class="sxs-lookup"><span data-stu-id="9973e-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="9973e-111">(наприклад, коли кілька одиниць додаються одночасно).</span><span class="sxs-lookup"><span data-stu-id="9973e-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="9973e-112">Робочі цикли не призначені для запуску в реальному часі, тому відповідну поведінку можна виконувати в режимі конструктора.</span><span class="sxs-lookup"><span data-stu-id="9973e-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="9973e-113">Якщо робочий цикл – це складна розширювана мова розмітки об'єктів (XMOL), то компіляцію може бути повільним.</span><span class="sxs-lookup"><span data-stu-id="9973e-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="9973e-114">Установіть прапорець у [цій](https://support.microsoft.com//kb/3043697) статті.</span><span class="sxs-lookup"><span data-stu-id="9973e-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="9973e-115">Ви повинні спростити робочий цикл або редизайн його за допомогою типу платформи робочого циклу Microsoft SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="9973e-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="9973e-116">Якщо журнал робочого циклу виріс великий, можливо, потрібно буде очистити елементи або створити новий список журналу.</span><span class="sxs-lookup"><span data-stu-id="9973e-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="9973e-117">Додаткові відомості: [очищення журналу робочого циклу](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="9973e-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="9973e-118">Пов’язані теми</span><span class="sxs-lookup"><span data-stu-id="9973e-118">Related topics</span></span>
<span data-ttu-id="9973e-119">Хочете спробувати Microsoft Flow у службі SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="9973e-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="9973e-120">Створення потоку</span><span class="sxs-lookup"><span data-stu-id="9973e-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="9973e-121">SharePoint і передавання</span><span class="sxs-lookup"><span data-stu-id="9973e-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


