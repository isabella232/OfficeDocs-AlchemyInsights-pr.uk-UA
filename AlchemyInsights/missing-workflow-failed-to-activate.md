---
title: Відсутні робочого процесу не вдалося активувати
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 44fd3c2d1e8b278b47c0fde6d48c7cbcbaa5c324
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543946"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="ea340-102">Відсутні робочого процесу не вдалося активувати</span><span class="sxs-lookup"><span data-stu-id="ea340-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="ea340-103">В колекції сайтів Microsoft SharePoint глобально для повторного використання робочого процесу (наприклад, "затвердження - SharePoint 2010") не можна додати до списку або бібліотеки.</span><span class="sxs-lookup"><span data-stu-id="ea340-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="ea340-104">Щоб вирішити цю проблему, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="ea340-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="ea340-105">Відкрити кореневий сайт колекції сайтів SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="ea340-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="ea340-106">Під **Сайт об'єктів**виберіть пункт **робочі процеси**.</span><span class="sxs-lookup"><span data-stu-id="ea340-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="ea340-107">У розділі **нової** стрічки **робочі процеси** виберіть **Багаторазового використання робочого процесу**.</span><span class="sxs-lookup"><span data-stu-id="ea340-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="ea340-108">У формі, **Створення багаторазового використання робочого процесу** , введіть ім'я \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="ea340-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="ea340-109">**Тип платформи**клацніть **Робочого циклу SharePoint 2010**і натисніть кнопку **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ea340-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="ea340-110">У **зберегти** розділі стрічки **робочого процесу** виберіть пункт **опублікувати**.</span><span class="sxs-lookup"><span data-stu-id="ea340-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="ea340-111">У розділі **керування** стрічки **робочий процес** виберіть **Опублікувати глобально**.</span><span class="sxs-lookup"><span data-stu-id="ea340-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="ea340-112">У діалоговому вікні підтвердження, що з'явиться виберіть **ОК**.</span><span class="sxs-lookup"><span data-stu-id="ea340-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="ea340-113">У веб-переглядачі, знайдіть кореневий сайт колекції сайтів та отримувати доступ до **Параметрів сайту** \> **Функцій колекції сайтів**.</span><span class="sxs-lookup"><span data-stu-id="ea340-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="ea340-114">Потім Увімкнути або вимкнути функцію **робочі процеси** :</span><span class="sxs-lookup"><span data-stu-id="ea340-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="ea340-115">· Якщо функція *активоване* , натисніть кнопку **Вимкнути** та натисніть кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="ea340-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="ea340-116">· Якщо функція *Deactivated* , натисніть кнопку **активувати**.</span><span class="sxs-lookup"><span data-stu-id="ea340-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="ea340-117">Для отримання додаткових відомостей зверніться до [статті](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="ea340-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

