---
title: SharePoint великі списки
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767306"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="344e2-102">Робота з великими списками та бібліотеками в SharePoint</span><span class="sxs-lookup"><span data-stu-id="344e2-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="344e2-103">Списки та бібліотеки SharePoint можуть містити до 30 000 000 елементів, але якщо вони мають більше 5 000 елементів, може відображатися граничне значення подання списку, помилка під час спроби працювати з ними.</span><span class="sxs-lookup"><span data-stu-id="344e2-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="344e2-104">Це граничне значення використовується для підтримання продуктивності служби.</span><span class="sxs-lookup"><span data-stu-id="344e2-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="344e2-105">Його не можна змінити.</span><span class="sxs-lookup"><span data-stu-id="344e2-105">It can't be changed.</span></span> <span data-ttu-id="344e2-106">Щоб уникнути попадання цього порогу:</span><span class="sxs-lookup"><span data-stu-id="344e2-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="344e2-107">**Використовувати сучасні**</span><span class="sxs-lookup"><span data-stu-id="344e2-107">**Use modern**</span></span>

<span data-ttu-id="344e2-108">Подання, що показують багато елементів, найкраще працюють у сучасному досвіді.</span><span class="sxs-lookup"><span data-stu-id="344e2-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="344e2-109">[Використовуйте сучасний досвід](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , щоб уникнути помилок, які можуть відображатися в класичному досвіді.</span><span class="sxs-lookup"><span data-stu-id="344e2-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="344e2-110">**Додати індекси**</span><span class="sxs-lookup"><span data-stu-id="344e2-110">**Add indexes**</span></span>

<span data-ttu-id="344e2-111">Під час фільтрування або сортування за стовпцем, який не має індексу, може відображатися повідомлення про помилку.</span><span class="sxs-lookup"><span data-stu-id="344e2-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="344e2-112">[Додайте покажчик](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) вручну з **параметрів списку** в меню налаштувань, потім **проіндексовані стовпці**.</span><span class="sxs-lookup"><span data-stu-id="344e2-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="344e2-113">**Редагування подання списку**</span><span class="sxs-lookup"><span data-stu-id="344e2-113">**Edit the list view**</span></span>

<span data-ttu-id="344e2-114">Якщо сталася помилка під час роботи з великим списком, [відредагуйте подання списку](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="344e2-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="344e2-115">Наступні чотири зміни призведе до видалення граничне значення подання списку помилок.</span><span class="sxs-lookup"><span data-stu-id="344e2-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="344e2-116">Внесіть усі чотири зміни, щоб видалити всі помилки.</span><span class="sxs-lookup"><span data-stu-id="344e2-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="344e2-117">Якщо ви все ще отримуєте помилки, перевірте [керування великими списками та бібліотеками](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="344e2-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="344e2-118">Виберіть **жоден** з обох **перших сортування за стовпцем** , а **потім Відсортуйте стовпець**.</span><span class="sxs-lookup"><span data-stu-id="344e2-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="344e2-119">Виберіть **жоден** з обох **перших груп за стовпцем** , а **потім згрупуйте за стовпцем**.</span><span class="sxs-lookup"><span data-stu-id="344e2-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="344e2-120">Виберіть **немає** для всіх стовпців у розділі **підсумки** .</span><span class="sxs-lookup"><span data-stu-id="344e2-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="344e2-121">Скасуйте вибір всього, окрім одного стовпчика для відображення з розділу **стовпці** .</span><span class="sxs-lookup"><span data-stu-id="344e2-121">Deselect all but one column for display from the **Columns** section.</span></span>

