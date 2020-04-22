---
title: Визначення активності правила для папки "Вхідні" в журналах аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716445"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="05d35-102">Визначення активності правила для папки "Вхідні" в журналах аудиту</span><span class="sxs-lookup"><span data-stu-id="05d35-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="05d35-103">Пошук журналу аудиту можна використовувати в центрі забезпечення безпеки & Microsoft 365, щоб переглянути події правила для папки "Вхідні" (створення, змінення та видалення правил для папки "Вхідні").</span><span class="sxs-lookup"><span data-stu-id="05d35-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="05d35-104">Увійдіть до [Microsoft 365 безпеки & центр відповідності](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="05d35-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="05d35-105">Перейдіть на сторінку **Search** > **пошуку журналу аудиту** пошуку.</span><span class="sxs-lookup"><span data-stu-id="05d35-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="05d35-106">Виберіть діапазон дат у полях Дата **початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="05d35-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="05d35-107">У розділі **справи поштової скриньки Exchange**переконайтеся, що поле **справи** встановлено на **новий-inboxrule створити/змінити/увімкнути/вимкнути правило для папки "Вхідні"**.</span><span class="sxs-lookup"><span data-stu-id="05d35-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="05d35-108">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="05d35-108">Click **Search**.</span></span>

<span data-ttu-id="05d35-109">У результатах пошуку виберіть запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="05d35-109">In the results, select an audit record.</span></span> <span data-ttu-id="05d35-110">У спливаючому меню відомості натисніть кнопку **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="05d35-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="05d35-111">Відомості про параметри правила для папки «Вхідні» відображаються в полі « **Параметри** ».</span><span class="sxs-lookup"><span data-stu-id="05d35-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="05d35-112">Щоб отримати додаткові відомості див. [визначення, якщо користувач створив правило для папки "Вхідні"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="05d35-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
