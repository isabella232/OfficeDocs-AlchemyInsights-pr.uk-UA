---
title: Великі списки SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720154"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="74fb4-102">Робота з великими списками та бібліотеками в SharePoint</span><span class="sxs-lookup"><span data-stu-id="74fb4-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="74fb4-103">Списки та бібліотеки SharePoint можуть містити до 30 000 000 елементи, але коли вони мають більше 5 000, може з'явитися повідомлення про поріг подання списку, коли ви намагаєтеся працювати з ними.</span><span class="sxs-lookup"><span data-stu-id="74fb4-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="74fb4-104">Це граничне значення використовується для підтримання продуктивності служби.</span><span class="sxs-lookup"><span data-stu-id="74fb4-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="74fb4-105">Його не можна змінити.</span><span class="sxs-lookup"><span data-stu-id="74fb4-105">It can't be changed.</span></span> <span data-ttu-id="74fb4-106">Щоб уникнути удару цього порогу, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="74fb4-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="74fb4-107">**Використання сучасної**</span><span class="sxs-lookup"><span data-stu-id="74fb4-107">**Use modern**</span></span>

<span data-ttu-id="74fb4-108">Подання, які відображають багато деталей, найкращим чином працюють в сучасному досвіді.</span><span class="sxs-lookup"><span data-stu-id="74fb4-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="74fb4-109">[Користуйтеся сучасним досвідом,](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) щоб уникнути помилок, які можуть відображатися в класичній версії.</span><span class="sxs-lookup"><span data-stu-id="74fb4-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="74fb4-110">**Додавання індексів**</span><span class="sxs-lookup"><span data-stu-id="74fb4-110">**Add indexes**</span></span>

<span data-ttu-id="74fb4-111">Під час фільтрування або сортування за стовпцем, який не має індексу, може з'явитися повідомлення про помилку.</span><span class="sxs-lookup"><span data-stu-id="74fb4-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="74fb4-112">[Додавання індексу](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) вручну з **параметрів списку** в меню "Параметри", а потім **індексованими стовпцями**.</span><span class="sxs-lookup"><span data-stu-id="74fb4-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="74fb4-113">**Редагування подання списку**</span><span class="sxs-lookup"><span data-stu-id="74fb4-113">**Edit the list view**</span></span>

<span data-ttu-id="74fb4-114">Якщо під час роботи з великим списком з'являється повідомлення про помилку, [Змініть подання списку](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="74fb4-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="74fb4-115">У наведених нижче чотирьох змін буде видалено помилки граничне значення подання списку.</span><span class="sxs-lookup"><span data-stu-id="74fb4-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="74fb4-116">Щоб видалити всі помилки, зробіть всі чотири зміни.</span><span class="sxs-lookup"><span data-stu-id="74fb4-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="74fb4-117">Якщо ви все одно одержуєте помилки, установіть прапорець [керувати великими списками та бібліотеками](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="74fb4-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="74fb4-118">Виберіть пункт **немає** з **першого сортування за стовпцем** , а **потім Відсортуйте його за стовпцем**.</span><span class="sxs-lookup"><span data-stu-id="74fb4-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="74fb4-119">Виберіть пункт **немає** в обох **перших групах за стовпцем** , а **потім – за стовпцем**.</span><span class="sxs-lookup"><span data-stu-id="74fb4-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="74fb4-120">У розділі " **підсумки** " виберіть пункт " **немає** " для всіх стовпців.</span><span class="sxs-lookup"><span data-stu-id="74fb4-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="74fb4-121">Вимкніть параметр "Усі", але один стовпець для відображення з розділу " **стовпці** ".</span><span class="sxs-lookup"><span data-stu-id="74fb4-121">Deselect all but one column for display from the **Columns** section.</span></span>

