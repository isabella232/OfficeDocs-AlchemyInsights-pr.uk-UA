---
title: Визначення подій видалення повідомлень у журналах аудиту
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696534"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="b7891-102">Журнали аудиту для видалених повідомлень електронної пошти</span><span class="sxs-lookup"><span data-stu-id="b7891-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="b7891-103">Починаючи з січня 2019, корпорація Майкрософт активування журналювання аудиту поштових скриньок за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="b7891-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="b7891-104">В іншому випадку, щоб переглянути повідомлення про видалення подій певного користувача, потрібно вручну ввімкнути видалення дій для аудиту.</span><span class="sxs-lookup"><span data-stu-id="b7891-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="b7891-105">Якщо журналювання аудиту поштової скриньки вже ввімкнуто для вашої організації або для певного користувача, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="b7891-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="b7891-106">Увійдіть у [центр відповідності & безпеки Microsoft 365](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b7891-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b7891-107">Натисніть кнопку **Пошук і дослідження** та виберіть пункт **Пошук у журналі аудиту**.</span><span class="sxs-lookup"><span data-stu-id="b7891-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="b7891-108">Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="b7891-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="b7891-109">Укажіть ім'я користувача для користувача, який потрібно дослідити (користувач, який видалив елементи).</span><span class="sxs-lookup"><span data-stu-id="b7891-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="b7891-110">У полі **дії** виберіть пункт **Видалені повідомлення з папки "Видалені** " та **переміщено повідомлення до папки "Видалені**".</span><span class="sxs-lookup"><span data-stu-id="b7891-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="b7891-111">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="b7891-111">Click **Search**.</span></span>

<span data-ttu-id="b7891-112">У результатах виберіть запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="b7891-112">In the results, select an audit record.</span></span> <span data-ttu-id="b7891-113">У розділі відомості про подробиці виберіть пункт **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="b7891-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b7891-114">Додаткові відомості про видалений елемент (наприклад, рядок теми та розташування елемента, коли його видалено) відображається в полі **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="b7891-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="b7891-115">Властивість **Clieninfostring** покаже, якщо видалення відбулося в програмі Outlook, Інтернет-версії Outlook (колишня назва – веб-програма Outlook Web App) або будь-який інший пристрій.</span><span class="sxs-lookup"><span data-stu-id="b7891-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="b7891-116">Докладні відомості наведено в статті [визначення користувачів, які настроїли пересилання електронної пошти для поштової скриньки](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="b7891-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="b7891-117">**Примітка**. не можна відновити видалені елементи за допомогою функції журналу аудиту.</span><span class="sxs-lookup"><span data-stu-id="b7891-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="b7891-118">Щоб відновити видалені повідомлення в Інтернет-версії Outlook, перегляньте статтю [відновлення видалених елементів у веб-програмі Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="b7891-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
