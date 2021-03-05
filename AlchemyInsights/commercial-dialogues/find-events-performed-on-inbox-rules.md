---
title: Пошуку подій, які виконуються в правилах для папки "Вхідні"
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483708"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="dff0b-102">Пошуку подій, які виконуються в правилах для папки "Вхідні"</span><span class="sxs-lookup"><span data-stu-id="dff0b-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="dff0b-103">Під час створення, змінення або видалення правил папки "Вхідні" події записуються в журнал аудиту.</span><span class="sxs-lookup"><span data-stu-id="dff0b-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="dff0b-104">Ось як можна переглянути їх.</span><span class="sxs-lookup"><span data-stu-id="dff0b-104">Here's how to review them:</span></span>

1. <span data-ttu-id="dff0b-105">Перейдіть до [центру відповідності & безпеки Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="dff0b-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="dff0b-106">Виберіть Пошук > пошуку в журналі аудиту.</span><span class="sxs-lookup"><span data-stu-id="dff0b-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="dff0b-107">Якщо відображається повідомлення про те, що потрібно ввімкнути відстеження, перейдіть вперед і ввімкніть її зараз.</span><span class="sxs-lookup"><span data-stu-id="dff0b-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="dff0b-108">Якщо цю функцію не ввімкнуто, результати пошуку не зможуть витягнути дані з попередніх дат.</span><span class="sxs-lookup"><span data-stu-id="dff0b-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="dff0b-109">Виберіть поле дії та знайдіть дії поштової скриньки Exchange, а потім виберіть New-InboxRule створити правило для папки "Вхідні" з веб-програми Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="dff0b-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="dff0b-110">Коли все буде Готово, клацніть за межі області, щоб згорнути область "дії".</span><span class="sxs-lookup"><span data-stu-id="dff0b-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="dff0b-111">Укажіть проміжок часу, а потім у полі користувачі виберіть ім'я користувача, яке потрібно дослідити.</span><span class="sxs-lookup"><span data-stu-id="dff0b-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="dff0b-112">Ви можете вибрати кілька користувачів за один раз.</span><span class="sxs-lookup"><span data-stu-id="dff0b-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="dff0b-113">Виберіть елемент пошук.</span><span class="sxs-lookup"><span data-stu-id="dff0b-113">Select Search.</span></span> <span data-ttu-id="dff0b-114">Дії відображаються в розділі результати.</span><span class="sxs-lookup"><span data-stu-id="dff0b-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="dff0b-115">Щоб переглянути відомості, виберіть потрібну дію, а потім виберіть пункт Додаткові відомості.</span><span class="sxs-lookup"><span data-stu-id="dff0b-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="dff0b-116">У розділі "Параметри" можна побачити ім'я правила, набір умов і дії, які потрібно виконати правилом.</span><span class="sxs-lookup"><span data-stu-id="dff0b-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="dff0b-117">Докладні відомості наведено в статті пошук у журналі аудиту Office 365 для виправлення поширених сценаріїв.</span><span class="sxs-lookup"><span data-stu-id="dff0b-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>