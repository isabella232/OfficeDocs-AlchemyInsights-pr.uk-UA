---
title: Виявлення події видалення повідомлення в журналах аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509009"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="72f51-102">Журнали аудиту для видалених повідомлень електронної пошти</span><span class="sxs-lookup"><span data-stu-id="72f51-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="72f51-103">Починаючи з січня 2019, корпорація Майкрософт вмикається журналювання аудиту поштових скриньок за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="72f51-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="72f51-104">В іншому випадку, щоб переглянути події видалення повідомлень для певного користувача, потрібно вручну ввімкнути видалення дій для відстеження.</span><span class="sxs-lookup"><span data-stu-id="72f51-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="72f51-105">Якщо журналювання аудиту поштової скриньки вже ввімкнуто для вашої організації або для конкретного користувача, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="72f51-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="72f51-106">Увійдіть до [Microsoft 365 безпеки & центр відповідності](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="72f51-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="72f51-107">Натисніть **Пошук і розслідування** , а потім виберіть **Пошук журналу перевірок**.</span><span class="sxs-lookup"><span data-stu-id="72f51-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="72f51-108">Виберіть діапазон дат у полях Дата **початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="72f51-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="72f51-109">Вкажіть ім'я користувача для користувача, який потрібно дослідити (користувач, який видалив елементи).</span><span class="sxs-lookup"><span data-stu-id="72f51-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="72f51-110">У полі **справи** виберіть пункт **Видалені повідомлення з папки "Видалені"** та **переміщено повідомлення до папки "Видалені"**.</span><span class="sxs-lookup"><span data-stu-id="72f51-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="72f51-111">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="72f51-111">Click **Search**.</span></span>

<span data-ttu-id="72f51-112">У результатах пошуку виберіть запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="72f51-112">In the results, select an audit record.</span></span> <span data-ttu-id="72f51-113">У спливаючому меню відомості натисніть кнопку **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="72f51-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="72f51-114">Додаткові відомості про видалений елемент (наприклад, рядок теми та розташування елемента, коли він був видалений) відображається в полі **Affecteditems** .</span><span class="sxs-lookup"><span data-stu-id="72f51-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="72f51-115">Властивість **клієнто** буде відображатися, якщо видалення відбулося в Outlook, Outlook в Інтернеті (раніше відомий як веб-застосунок Outlook Web App) або будь-який інший пристрій.</span><span class="sxs-lookup"><span data-stu-id="72f51-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="72f51-116">Для отримання додаткових відомостей див. [визначення, які встановлюють пересилання електронної пошти для поштової скриньки](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="72f51-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="72f51-117">**Примітка**: ви не можете відновити видалені елементи за допомогою функції журналу аудиту.</span><span class="sxs-lookup"><span data-stu-id="72f51-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="72f51-118">Щоб відновити видалені повідомлення в Outlook, в Інтернеті, перегляньте статтю [відновлення видалених елементів у веб-застосунку Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="72f51-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
