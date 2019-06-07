---
title: Визначити пересилання зовнішніх електронної пошти поштових скриньок у журнали аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1369
ms.assetid: ''
ms.openlocfilehash: 518e4dd485ee7c54ce83e65794152e32f4c3a836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752042"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="ea488-102">Визначити коли пересилання електронної пошти зовнішніх налаштовано на поштові скриньки</span><span class="sxs-lookup"><span data-stu-id="ea488-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="ea488-103">Коли користувач налаштовує пересилання зовнішніх електронної пошти в поштовій скриньці, діяльність аудит як частину на командлета **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="ea488-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="ea488-104">Ви можете побачити діяльності, використовуючи пошук журналу аудиту у безпеки & центрі дотримання.</span><span class="sxs-lookup"><span data-stu-id="ea488-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="ea488-105">Увійдіть до [Office 365 безпеки & відповідно центр](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="ea488-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="ea488-106">Натисніть кнопку **Пошук та розслідування** та виберіть **Пошук журналу аудиту**.</span><span class="sxs-lookup"><span data-stu-id="ea488-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="ea488-107">Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="ea488-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="ea488-108">Вам не потрібно вказати ім'я користувача.</span><span class="sxs-lookup"><span data-stu-id="ea488-108">You don't need to specify a username.</span></span> <span data-ttu-id="ea488-109">Перевірте, чи **діяльність** поля вибрано **відображення результатів для всіх видів діяльності**.</span><span class="sxs-lookup"><span data-stu-id="ea488-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="ea488-110">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="ea488-110">Click **Search**.</span></span>

<span data-ttu-id="ea488-111">В результатах пошуку клацніть **Фільтр результатів** і введіть **Set-Mailbox** у поле фільтр діяльності.</span><span class="sxs-lookup"><span data-stu-id="ea488-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="ea488-112">Виберіть запис аудиту в результатах пошуку.</span><span class="sxs-lookup"><span data-stu-id="ea488-112">Select an audit record in the results.</span></span> <span data-ttu-id="ea488-113">У **деталі** спливаюче виберіть **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="ea488-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="ea488-114">Ви повинні дивитися на деталі кожної аудиту запису, щоб визначити, якщо діяльність пов'язана з електронною поштою пересилання.</span><span class="sxs-lookup"><span data-stu-id="ea488-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="ea488-115">**ObjectId**: псевдонім значення поштової скриньки, яку було змінено.</span><span class="sxs-lookup"><span data-stu-id="ea488-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="ea488-116">**Параметри**: _ForwardingSmtpAddress_ вказує цільову адресу електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="ea488-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="ea488-117">**Ім'я користувача**: користувач, який налаштований пересилання електронної пошти для поштової скриньки в **ObjectId** області.</span><span class="sxs-lookup"><span data-stu-id="ea488-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="ea488-118">Докладніше перегляньте [Determining, яка настроювала електронної пошти пересилання для поштової скриньки](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="ea488-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
