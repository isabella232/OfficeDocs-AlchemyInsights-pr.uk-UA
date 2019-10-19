---
title: Відсутній робочий цикл не вдалося активувати
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36753817"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="83587-102">Відсутній робочий цикл не вдалося активувати</span><span class="sxs-lookup"><span data-stu-id="83587-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="83587-103">У колекції сайтів Microsoft SharePoint не можна додати глобальний робочий цикл для повторного використання (наприклад, "затвердження-SharePoint 2010") до списку або бібліотеки.</span><span class="sxs-lookup"><span data-stu-id="83587-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="83587-104">Щоб вирішити цю проблему, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="83587-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="83587-105">Відкрийте кореневий веб-сайт колекції сайтів у SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="83587-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="83587-106">У розділі **об'єкти сайту**виберіть **робочі процеси**.</span><span class="sxs-lookup"><span data-stu-id="83587-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="83587-107">У **новому** розділі стрічки **робочих циклів** виберіть **робочий цикл багаторазового використання**.</span><span class="sxs-lookup"><span data-stu-id="83587-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="83587-108">У формі **створення багаторазового робочого циклу** введіть ім'я \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="83587-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="83587-109">**Тип платформи**, клацніть **робочий цикл SharePoint 2010**і натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="83587-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="83587-110">У розділі **збереження** стрічки **робочого циклу** виберіть **опублікувати**.</span><span class="sxs-lookup"><span data-stu-id="83587-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="83587-111">У розділі **керування** стрічки **робочого циклу** виберіть **опублікувати глобально**.</span><span class="sxs-lookup"><span data-stu-id="83587-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="83587-112">У діалоговому вікні підтвердження, що з'явиться, натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="83587-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="83587-113">У веб-переглядачі знайдіть кореневий веб-сайт колекції сайтів, а потім перейдіть до **параметрів** \> **колекції**сайтів.</span><span class="sxs-lookup"><span data-stu-id="83587-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="83587-114">Після цього переклюніть функцію **робочі цикли** :</span><span class="sxs-lookup"><span data-stu-id="83587-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="83587-115">· Якщо цю функцію *активовано* , натисніть кнопку **деактивувати,** а потім натисніть кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="83587-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="83587-116">· Якщо цю функцію *вимкнено* , натисніть кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="83587-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="83587-117">Для отримання додаткової інформації, будь ласка, зверніться до наступній [статті](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="83587-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

