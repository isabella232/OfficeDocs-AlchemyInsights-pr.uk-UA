---
title: Визначити «вхідні» правилом активності в журнали аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: f130846dd24cef81177934aa2a200c1056172d3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755058"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="818e9-102">Визначити «вхідні» правилом активності в журнали аудиту</span><span class="sxs-lookup"><span data-stu-id="818e9-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="818e9-103">За допомогою пошуку журналу аудиту безпеки & відповідно центр для перегляду папки «Вхідні» правилом події (створення, редагування та видалення папки Вхідні правила).</span><span class="sxs-lookup"><span data-stu-id="818e9-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="818e9-104">Увійдіть до [Office 365 безпеки & відповідно центр](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="818e9-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="818e9-105">Натисніть кнопку **Пошук та розслідування** та виберіть **Пошук журналу аудиту**.</span><span class="sxs-lookup"><span data-stu-id="818e9-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="818e9-106">Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="818e9-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="818e9-107">За **Діяльність поштової скриньки Exchange**перевірте, чи **діяльність** поля має значення **Нью-InboxRule створити/змінити/увімкнути/вимкнути правило для вхідних повідомлень**.</span><span class="sxs-lookup"><span data-stu-id="818e9-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="818e9-108">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="818e9-108">Click **Search**.</span></span>

<span data-ttu-id="818e9-109">В результатах пошуку виберіть запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="818e9-109">In the results, select an audit record.</span></span> <span data-ttu-id="818e9-110">У деталі спливаюче виберіть **Більше інформації**.</span><span class="sxs-lookup"><span data-stu-id="818e9-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="818e9-111">Інформацію про параметри правило папки «Вхідні» відображається в області **параметрів** .</span><span class="sxs-lookup"><span data-stu-id="818e9-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="818e9-112">Докладніше перегляньте [Determining, якщо користувач створив правило для вхідних повідомлень](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="818e9-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
