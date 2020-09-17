---
title: Визначення дії правила для папки "Вхідні" в журналах аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779072"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="494b5-102">Визначення дії правила для папки "Вхідні" в журналах аудиту</span><span class="sxs-lookup"><span data-stu-id="494b5-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="494b5-103">Ви можете використовувати пошук у журналі аудиту в центрі відповідності & безпеки Microsoft 365, щоб переглянути події правила для папки "Вхідні" (створення, змінення та видалення правил для папки "Вхідні").</span><span class="sxs-lookup"><span data-stu-id="494b5-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="494b5-104">Увійдіть у [центр відповідності & безпеки Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="494b5-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="494b5-105">Перейдіть на сторінку **Search**  >  **Пошук журналу аудиту** .</span><span class="sxs-lookup"><span data-stu-id="494b5-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="494b5-106">Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="494b5-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="494b5-107">У розділі **дії поштової скриньки Exchange**переконайтеся, що в полі " **дії** " настроєно значення **"створити" або "змінити", щоб установити або вимкнути правило папки "Вхідні"**.</span><span class="sxs-lookup"><span data-stu-id="494b5-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="494b5-108">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="494b5-108">Click **Search**.</span></span>

<span data-ttu-id="494b5-109">У результатах виберіть запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="494b5-109">In the results, select an audit record.</span></span> <span data-ttu-id="494b5-110">У розділі відомості про подробиці виберіть пункт **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="494b5-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="494b5-111">Відомості про настройки правила для папки "Вхідні" відображаються в полі " **Параметри** ".</span><span class="sxs-lookup"><span data-stu-id="494b5-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="494b5-112">Докладні відомості наведено в статті [визначення того, чи користувач створив правило для папки "Вхідні"](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule) .</span><span class="sxs-lookup"><span data-stu-id="494b5-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
