---
title: Визначити видалити повідомлення події в журнали аудиту
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416730"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="bb745-102">Журнали аудиту для видалені повідомлення електронної пошти</span><span class="sxs-lookup"><span data-stu-id="bb745-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="bb745-103">Починаючи з січня 2019 року Microsoft ввімкнути журналювання за промовчанням аудиту поштових скриньок.</span><span class="sxs-lookup"><span data-stu-id="bb745-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="bb745-104">В іншому випадку, переглядати події видалити повідомлення певного користувача, необхідно вручну включити дії delete для аудиту.</span><span class="sxs-lookup"><span data-stu-id="bb745-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="bb745-105">Якщо поштова скринька аудиту вже вмикається для вашої організації або для певного користувача, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="bb745-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="bb745-106">Увійдіть до [Office 365 безпеки & відповідно центр](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="bb745-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="bb745-107">Натисніть кнопку **Пошук та розслідування** та виберіть **Пошук журналу аудиту**.</span><span class="sxs-lookup"><span data-stu-id="bb745-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="bb745-108">Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="bb745-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="bb745-109">Укажіть ім'я користувача для користувача, якого ви хочете, щоб розслідувати (користувача, який видалені елементи).</span><span class="sxs-lookup"><span data-stu-id="bb745-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="bb745-110">У сфері **діяльності** виберіть **Видалені повідомлення з папки "Видалені"** а **повідомлення переміщено до папки "Видалені"**.</span><span class="sxs-lookup"><span data-stu-id="bb745-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="bb745-111">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="bb745-111">Click **Search**.</span></span>

<span data-ttu-id="bb745-112">В результатах пошуку виберіть запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="bb745-112">In the results, select an audit record.</span></span> <span data-ttu-id="bb745-113">У деталі спливаюче виберіть **Більше інформації**.</span><span class="sxs-lookup"><span data-stu-id="bb745-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="bb745-114">Додаткові відомості про видалений елемент (наприклад, рядок теми і розташування об'єкта, коли його було видалено) відображається в області **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="bb745-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="bb745-115">Властивість **ClientInfoString** покаже, якщо видалення стався в Outlook, Outlook web (раніше відомий як веб-застосунок Outlook Web App) або будь-якого іншого пристрою.</span><span class="sxs-lookup"><span data-stu-id="bb745-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="bb745-116">Докладніше перегляньте [Determining, яка настроювала електронної пошти пересилання для поштової скриньки](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="bb745-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="bb745-117">**Примітка**: не вдалося отримати видалені елементи за допомогою функції журналу аудиту.</span><span class="sxs-lookup"><span data-stu-id="bb745-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="bb745-118">Щоб відновити видалені повідомлення в Outlook, в Інтернеті, див [відновити видалені елементи у веб-застосунку Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="bb745-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
