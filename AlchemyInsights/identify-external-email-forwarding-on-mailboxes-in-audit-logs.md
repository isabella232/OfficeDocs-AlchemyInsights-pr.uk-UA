---
title: Визначення зовнішньої пересилання електронної пошти на поштові скриньки в журналах аудиту
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696318"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="ee364-102">Визначення того, що для поштових скриньок настроєно зовнішнє пересилання електронної пошти</span><span class="sxs-lookup"><span data-stu-id="ee364-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="ee364-103">Коли користувач Microsoft 365 настроює зовнішню пересилання електронної пошти в поштовій скриньці, дія перевіряється як частину командлета **Set-Mailbox** .</span><span class="sxs-lookup"><span data-stu-id="ee364-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="ee364-104">Ви можете переглянути дії за допомогою функції пошуку в журналі аудиту в центрі відповідності & безпеки.</span><span class="sxs-lookup"><span data-stu-id="ee364-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="ee364-105">Увійдіть у [центр відповідності & безпеки Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="ee364-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="ee364-106">Перейдіть на сторінку **Search**  >  **Пошук журналу аудиту** .</span><span class="sxs-lookup"><span data-stu-id="ee364-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="ee364-107">Виберіть діапазон дат у полях **Дата початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="ee364-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="ee364-108">Не потрібно вказувати ім'я користувача.</span><span class="sxs-lookup"><span data-stu-id="ee364-108">You don't need to specify a username.</span></span> <span data-ttu-id="ee364-109">Переконайтеся, що поле " **дії** " настроєно для **відображення результатів для всіх дій**.</span><span class="sxs-lookup"><span data-stu-id="ee364-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="ee364-110">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="ee364-110">Click **Search**.</span></span>

<span data-ttu-id="ee364-111">У результатах пошуку клацніть елемент **Фільтрувати результати** та введіть у полі фільтра дій **набір – поштова скринька** .</span><span class="sxs-lookup"><span data-stu-id="ee364-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="ee364-112">Виберіть запис аудиту в результатах.</span><span class="sxs-lookup"><span data-stu-id="ee364-112">Select an audit record in the results.</span></span> <span data-ttu-id="ee364-113">У розділі **відомості про подробиці** виберіть пункт **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="ee364-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="ee364-114">Щоб визначити, чи пов'язані дії з пересиланням електронної пошти, потрібно переглянути відомості про кожний запис аудиту.</span><span class="sxs-lookup"><span data-stu-id="ee364-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="ee364-115">**Об'єктивна**: псевдонім поштової скриньки, яку було змінено.</span><span class="sxs-lookup"><span data-stu-id="ee364-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="ee364-116">**Параметри**: _адреса_ електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="ee364-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="ee364-117">**Userid**: користувач, який налаштував пересилання електронної пошти на поштову скриньку в полі " **об'єктивність** ".</span><span class="sxs-lookup"><span data-stu-id="ee364-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="ee364-118">Докладні відомості наведено в статті [визначення користувачів, які настроїли пересилання електронної пошти для поштової скриньки](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="ee364-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
