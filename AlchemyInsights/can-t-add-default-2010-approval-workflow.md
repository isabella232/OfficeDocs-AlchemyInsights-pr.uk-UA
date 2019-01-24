---
title: Не можна додати за промовчанням робочий процес затвердження 2010
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29495389"
---
# <a name="cant-add-default-2010-approval-workflow"></a><span data-ttu-id="33402-102">Не можна додати за промовчанням робочий процес затвердження 2010</span><span class="sxs-lookup"><span data-stu-id="33402-102">Can't add default 2010 Approval Workflow</span></span>

<span data-ttu-id="33402-103">В колекції сайтів Microsoft SharePoint глобально для повторного використання робочого процесу (наприклад, "затвердження - SharePoint 2010") не можна додати до списку або бібліотеки.</span><span class="sxs-lookup"><span data-stu-id="33402-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="33402-104">Щоб вирішити цю проблему, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="33402-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="33402-105">Відкрити кореневий сайт колекції сайтів SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="33402-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="33402-106">Під **Сайт об'єктів**виберіть пункт **робочі процеси**.</span><span class="sxs-lookup"><span data-stu-id="33402-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="33402-107">У розділі **нової** стрічки **робочі процеси** виберіть **Багаторазового використання робочого процесу**.</span><span class="sxs-lookup"><span data-stu-id="33402-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="33402-p101">У формі, **Створення багаторазового використання робочого процесу** , введіть ім'я \* \*\*Repair2010\*\*\*. **Тип платформи**оберіть **Робочого циклу SharePoint 2010**та клацніть **OK**.</span><span class="sxs-lookup"><span data-stu-id="33402-p101">On the **Create Reusable Workflow** form, enter the name  \* **Repair2010**\* . For **Platform Type**, select **SharePoint 2010 Workflow**, and then select **OK**.</span></span> 
  
5. <span data-ttu-id="33402-110">У **зберегти** розділі стрічки **робочого процесу** виберіть пункт **опублікувати**.</span><span class="sxs-lookup"><span data-stu-id="33402-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
6. <span data-ttu-id="33402-p102">У розділі **керування** стрічки **робочий процес** виберіть **Опублікувати глобально**. У діалоговому вікні підтвердження, що з'явиться виберіть **ОК**.</span><span class="sxs-lookup"><span data-stu-id="33402-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
7. <span data-ttu-id="33402-p103">У веб-переглядачі, знайдіть кореневий сайт колекції сайтів та отримувати доступ до **Параметрів сайту** \> **Функцій колекції сайтів**. Потім Увімкнути або вимкнути функцію **робочі процеси** :</span><span class="sxs-lookup"><span data-stu-id="33402-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="33402-115">· Якщо функція *активоване* , натисніть кнопку **Вимкнути** та натисніть кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="33402-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="33402-116">· Якщо функція *Deactivated* , натисніть кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="33402-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="33402-117">Для отримання додаткових відомостей зверніться до [статті](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="33402-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

