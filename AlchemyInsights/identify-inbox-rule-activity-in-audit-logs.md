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
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539194"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="f67f4-102">Визначити «вхідні» правилом активності в журнали аудиту</span><span class="sxs-lookup"><span data-stu-id="f67f4-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="f67f4-103">Дає змогу аудиту журнал пошуку в Office 365 безпеки & центрі дотримання переглядати вхідні правила події (створення, редагування та видалення папки Вхідні правила).</span><span class="sxs-lookup"><span data-stu-id="f67f4-103">You can use audit log search in the Office 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="f67f4-104">Увійдіть до [Office 365 безпеки & центрі дотримання](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="f67f4-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="f67f4-105">Перейти до **пошуку** > сторінку**пошуку журналу аудиту** .</span><span class="sxs-lookup"><span data-stu-id="f67f4-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="f67f4-106">Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="f67f4-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="f67f4-107">За **Діяльність поштової скриньки Exchange**перевірте, чи **діяльність** поля має значення **Нью-InboxRule створити/змінити/увімкнути/вимкнути правило для вхідних повідомлень**.</span><span class="sxs-lookup"><span data-stu-id="f67f4-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="f67f4-108">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="f67f4-108">Click **Search**.</span></span>

<span data-ttu-id="f67f4-109">В результатах пошуку виберіть запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="f67f4-109">In the results, select an audit record.</span></span> <span data-ttu-id="f67f4-110">У деталі спливаюче виберіть **Більше інформації**.</span><span class="sxs-lookup"><span data-stu-id="f67f4-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f67f4-111">Інформацію про параметри правило папки «Вхідні» відображається в області **параметрів** .</span><span class="sxs-lookup"><span data-stu-id="f67f4-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="f67f4-112">Докладніше перегляньте [Determining, якщо користувач створив правило для вхідних повідомлень](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="f67f4-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
