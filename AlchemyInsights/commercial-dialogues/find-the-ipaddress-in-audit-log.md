---
title: Визначення IP-адреси в журналі аудиту
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483713"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="f7c5e-102">Визначення IP-адреси в журналі аудиту</span><span class="sxs-lookup"><span data-stu-id="f7c5e-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="f7c5e-103">IP-адреса, що відповідає діяльності, що виконується користувачем або адміністратором, відображається в журналах аудиту.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="f7c5e-104">Відомості про клієнта також записуються.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-104">The client information is also logged.</span></span> <span data-ttu-id="f7c5e-105">Ось як можна визначити IP-адресу:</span><span class="sxs-lookup"><span data-stu-id="f7c5e-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="f7c5e-106">Перейдіть до [центру відповідності & безпеки Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="f7c5e-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="f7c5e-107">Виберіть **пункт**  >  **[Пошук у журналі аудиту](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="f7c5e-108">Якщо відображається повідомлення про те, що потрібно ввімкнути відстеження, перейдіть вперед і ввімкніть її зараз.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="f7c5e-109">Якщо цю функцію не активовано, результати пошуку не зможуть витягнути дані з попередніх дат.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="f7c5e-110">Якщо вас цікавить певна дія, виберіть його зі списку **дії** ; в іншому разі за замовчуванням всі дії буде повернуто вибраному користувачу.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="f7c5e-111">Зверніть увагу, що деякі дії можуть бути недоступні для вибраного в меню " **дії** ". Проте ці елементи аудиту буде повернуто, якщо вибрано параметр **Відображати результати для всіх дій** (Настроювання за замовчуванням).</span><span class="sxs-lookup"><span data-stu-id="f7c5e-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="f7c5e-112">Укажіть проміжок часу, а потім у полі **користувачі** виберіть ім'я користувача, яке потрібно дослідити.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="f7c5e-113">Виберіть елемент **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-113">Select **Search**.</span></span> <span data-ttu-id="f7c5e-114">Дії відображаються в розділі **результати**.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-114">The activities appear under **Results**.</span></span> <span data-ttu-id="f7c5e-115">IP-адресу для кожної дії можна переглянути.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="f7c5e-116">Щоб переглянути відомості, виберіть потрібну дію, а потім виберіть пункт **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="f7c5e-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="f7c5e-117">Докладні відомості наведено в статті пошук у [журналі аудиту Office 365 для виправлення поширених сценаріїв](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="f7c5e-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>