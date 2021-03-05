---
title: Дізнайтеся, кому настроєно пересилання в поштовій скриньці, а також про те, як
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483358"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="de942-102">Дізнайтеся, кому настроєно пересилання в поштовій скриньці, а також про те, як</span><span class="sxs-lookup"><span data-stu-id="de942-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="de942-103">Якщо для поштової скриньки установлено зовнішню переадресацію, дія перевіряється як частину Set-Mailbox командлет.</span><span class="sxs-lookup"><span data-stu-id="de942-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="de942-104">Ось як можна відшукати дії в журналі аудиту.</span><span class="sxs-lookup"><span data-stu-id="de942-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="de942-105">Перейдіть до [центру відповідності & безпеки Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="de942-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="de942-106">Виберіть **пункт** >  **Пошук у журналі аудиту**.</span><span class="sxs-lookup"><span data-stu-id="de942-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="de942-107">Якщо відображається повідомлення про те, що потрібно ввімкнути відстеження, перейдіть вперед і ввімкніть її зараз.</span><span class="sxs-lookup"><span data-stu-id="de942-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="de942-108">Якщо цю функцію не ввімкнуто, результати пошуку не зможуть витягнути дані з попередніх дат.</span><span class="sxs-lookup"><span data-stu-id="de942-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="de942-109">Переконайтеся, що поле " **дії** " настроєно для **відображення результатів для всіх дій** (за замовчуванням).</span><span class="sxs-lookup"><span data-stu-id="de942-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="de942-110">Укажіть проміжок часу.</span><span class="sxs-lookup"><span data-stu-id="de942-110">Specify the date range.</span></span> <span data-ttu-id="de942-111">Не потрібно вказувати ім'я користувача.</span><span class="sxs-lookup"><span data-stu-id="de942-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="de942-112">Виберіть елемент **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="de942-112">Select **Search**.</span></span> <span data-ttu-id="de942-113">Дії відображаються в розділі **результати**.</span><span class="sxs-lookup"><span data-stu-id="de942-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="de942-114">Виберіть елемент **Фільтрувати результати**, а потім у полі фільтр **дій** введіть **Set-поштова скринька** .</span><span class="sxs-lookup"><span data-stu-id="de942-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="de942-115">Ця функція повертає всі дії зі **створення поштових скриньок** .</span><span class="sxs-lookup"><span data-stu-id="de942-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="de942-116">Щоб переглянути відомості, виберіть потрібну дію, а потім виберіть пункт **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="de942-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="de942-117">У розділі **Параметри** можна побачити адресу електронної пошти, яку було настроєно в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="de942-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="de942-118">**Userid** представляє користувача, який настроїла зовнішню переадресацію в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="de942-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="de942-119">Докладні відомості наведено в статті [Пошук у журналі аудиту Office 365 для виправлення поширених сценаріїв](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="de942-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>