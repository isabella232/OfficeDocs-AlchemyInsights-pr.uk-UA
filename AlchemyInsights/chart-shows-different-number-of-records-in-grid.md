---
title: Діаграма показує різну кількість записів у сітці
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439958"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="1a448-102">Діаграма показує різну кількість записів у сітці</span><span class="sxs-lookup"><span data-stu-id="1a448-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="1a448-103">**Симптом**</span><span class="sxs-lookup"><span data-stu-id="1a448-103">**Symptom**</span></span>

<span data-ttu-id="1a448-104">Для діаграми на сторінці приладної дошки, коли ви натискаєте на діаграмі "..." і натисніть "Переглянути записи", ви переходите до сітки сторінки, щоб побачити всі записи. Іноді кількість записів змінюється.</span><span class="sxs-lookup"><span data-stu-id="1a448-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="1a448-105">**Причиною**</span><span class="sxs-lookup"><span data-stu-id="1a448-105">**Cause**</span></span>

<span data-ttu-id="1a448-106">Це пов'язано з різницею подань між діаграмою на оригінальній сторінці приладної дошки та діаграми на головній сторінці сітки.</span><span class="sxs-lookup"><span data-stu-id="1a448-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="1a448-107">**Рішення**</span><span class="sxs-lookup"><span data-stu-id="1a448-107">**Solution**</span></span>

1. <span data-ttu-id="1a448-108">Перевірте подання з вихідної сторінки та подання в сітці, щоб побачити, якщо вони різні.</span><span class="sxs-lookup"><span data-stu-id="1a448-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="1a448-109">Змініть подання в сітці відповідно до подання на вихідній сторінці.</span><span class="sxs-lookup"><span data-stu-id="1a448-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="1a448-110">Якщо правильне подання не знайдено, зазвичай це означає, що подання не ввімкнуто в конструкторі програм.</span><span class="sxs-lookup"><span data-stu-id="1a448-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="1a448-111">Перейдіть до конструктора програм певної програми, виберіть сутність та її подання, перевірте подання, яке потрібно ввімкнути, зберегти, опублікувати та закрити.</span><span class="sxs-lookup"><span data-stu-id="1a448-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="1a448-112">Оновіть сторінку.</span><span class="sxs-lookup"><span data-stu-id="1a448-112">Refresh the page.</span></span>