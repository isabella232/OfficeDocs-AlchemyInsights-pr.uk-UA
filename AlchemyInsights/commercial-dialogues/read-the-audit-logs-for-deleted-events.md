---
title: Читання журналів аудиту для видалених подій
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483322"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="28f6b-102">Читання журналів аудиту для видалених подій</span><span class="sxs-lookup"><span data-stu-id="28f6b-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="28f6b-103">Ось як це зробити:</span><span class="sxs-lookup"><span data-stu-id="28f6b-103">Here's how to do this:</span></span>

1. <span data-ttu-id="28f6b-104">Перейдіть до [центру відповідності & безпеки Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="28f6b-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="28f6b-105">Виберіть **пункт**  >  [**Пошук у журналі аудиту**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="28f6b-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="28f6b-106">Якщо відображається повідомлення про те, що потрібно ввімкнути функцію, перейдіть вперед і ввімкніть її зараз.</span><span class="sxs-lookup"><span data-stu-id="28f6b-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="28f6b-107">Якщо функцію не ввімкнуто, результати пошуку не зможуть витягнути дані з попередніх дат.</span><span class="sxs-lookup"><span data-stu-id="28f6b-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="28f6b-108">Виберіть елемент **дії**, а потім знайдіть **дії поштової скриньки Exchange**.</span><span class="sxs-lookup"><span data-stu-id="28f6b-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="28f6b-109">Виберіть **Видалені повідомлення з** папки "Видалені" та **переміщено повідомлення до** параметрів папки "Видалені".</span><span class="sxs-lookup"><span data-stu-id="28f6b-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="28f6b-110">Коли все буде Готово, клацніть за межі області, щоб згорнути область " **дії** ".</span><span class="sxs-lookup"><span data-stu-id="28f6b-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="28f6b-111">Укажіть проміжок часу, а потім у полі **користувачі** виберіть ім'я користувача, яке потрібно дослідити.</span><span class="sxs-lookup"><span data-stu-id="28f6b-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="28f6b-112">Ви можете вибрати кілька користувачів за один раз.</span><span class="sxs-lookup"><span data-stu-id="28f6b-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="28f6b-113">Виберіть елемент **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="28f6b-113">Select **Search**.</span></span> <span data-ttu-id="28f6b-114">Дії відображаються в розділі **результати**.</span><span class="sxs-lookup"><span data-stu-id="28f6b-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="28f6b-115">Щоб переглянути відомості, виберіть потрібну дію, а потім виберіть пункт **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="28f6b-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="28f6b-116">Додаткові відомості про видалений елемент, як-от рядок теми та розташування елемента, коли його видалено, буде відображено в полі **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="28f6b-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="28f6b-117">Не можна відновити видалені елементи за допомогою функції "журнал аудиту".</span><span class="sxs-lookup"><span data-stu-id="28f6b-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="28f6b-118">Щоб відновити видалені елементи, перегляньте статтю [відновлення видалених або електронних листів у веб-програмі Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="28f6b-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="28f6b-119">Докладні відомості наведено в статті [Пошук у журналі аудиту Office 365 для виправлення поширених сценаріїв](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="28f6b-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
