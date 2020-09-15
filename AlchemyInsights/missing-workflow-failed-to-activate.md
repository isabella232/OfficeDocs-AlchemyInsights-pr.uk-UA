---
title: Не вдалося активувати відсутній робочий цикл
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667107"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="3d228-102">Не вдалося активувати відсутній робочий цикл</span><span class="sxs-lookup"><span data-stu-id="3d228-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="3d228-103">У колекції сайтів Microsoft SharePoint не можна додати глобальний робочий цикл багаторазового використання (наприклад, "затвердження – SharePoint 2010") до списку або бібліотеки.</span><span class="sxs-lookup"><span data-stu-id="3d228-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="3d228-104">Щоб вирішити цю проблему, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="3d228-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="3d228-105">Відкрийте кореневий веб-сайт колекції сайтів у програмі SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="3d228-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="3d228-106">У розділі **об'єкти сайту**виберіть пункт **робочі цикли**.</span><span class="sxs-lookup"><span data-stu-id="3d228-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="3d228-107">У **новому** розділі стрічки **робочі цикли** натисніть кнопку **робочий цикл для повторного використання**.</span><span class="sxs-lookup"><span data-stu-id="3d228-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="3d228-108">У формі **робочого циклу створення багаторазових** введіть ім'я \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="3d228-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="3d228-109">Для **типу платформи**виберіть пункт **робочий цикл SharePoint 2010**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="3d228-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="3d228-110">У розділі **збереження** стрічки **робочого циклу** натисніть кнопку **опублікувати**.</span><span class="sxs-lookup"><span data-stu-id="3d228-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="3d228-111">У розділі **керування** на стрічці **робочого циклу** натисніть кнопку **опублікувати глобально**.</span><span class="sxs-lookup"><span data-stu-id="3d228-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="3d228-112">У діалоговому вікні підтвердження, що з'явиться, натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="3d228-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="3d228-113">У веб-браузері знайдіть кореневий веб-сайт колекції сайтів, а потім у розділі **Параметри** \> **колекції**сайтів Access.</span><span class="sxs-lookup"><span data-stu-id="3d228-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="3d228-114">Після цього переключати функцію **робочі цикли** .</span><span class="sxs-lookup"><span data-stu-id="3d228-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="3d228-115">· Якщо функцію  *активовано*  , натисніть кнопку **Вимкнути,** а потім – кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="3d228-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="3d228-116">· Якщо функцію  *деактивовано*  , натисніть кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="3d228-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="3d228-117">Щоб отримати докладніші відомості, ознайомтеся з наведеними нижче [статтею](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="3d228-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

