---
title: Визначення зовнішньої електронної пошти пересилання поштових скриньок у журналах аудиту
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508973"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="64133-102">Визначте, коли зовнішня пересилання електронної пошти налаштовано на поштових скриньках</span><span class="sxs-lookup"><span data-stu-id="64133-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="64133-103">Під час Microsoft 365 користувача, настроювання зовнішньої електронної пошти пересилання поштової скриньки, діяльність перевіряється, частина командлета **Set-поштової скриньки** .</span><span class="sxs-lookup"><span data-stu-id="64133-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="64133-104">Можна переглянути дії за допомогою пошуку журналу аудиту в центрі підтримки & відповідності.</span><span class="sxs-lookup"><span data-stu-id="64133-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="64133-105">Увійдіть до [Microsoft 365 безпеки & центр відповідності](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="64133-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="64133-106">Перейдіть на сторінку **Search**  >  **пошуку журналу аудиту** пошуку.</span><span class="sxs-lookup"><span data-stu-id="64133-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="64133-107">Виберіть діапазон дат у полях Дата **початку** та **Дата завершення** .</span><span class="sxs-lookup"><span data-stu-id="64133-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="64133-108">Вам не потрібно вказувати ім'я користувача.</span><span class="sxs-lookup"><span data-stu-id="64133-108">You don't need to specify a username.</span></span> <span data-ttu-id="64133-109">Переконайтеся, що поле **справи** налаштовано на **відображення результатів для всіх справ**.</span><span class="sxs-lookup"><span data-stu-id="64133-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="64133-110">Натисніть кнопку **Пошук**.</span><span class="sxs-lookup"><span data-stu-id="64133-110">Click **Search**.</span></span>

<span data-ttu-id="64133-111">У результатах пошуку натисніть кнопку **Фільтрувати результати** та введіть **набір-поштову скриньку** у полі фільтр активності.</span><span class="sxs-lookup"><span data-stu-id="64133-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="64133-112">Виберіть запис аудиту в результатах.</span><span class="sxs-lookup"><span data-stu-id="64133-112">Select an audit record in the results.</span></span> <span data-ttu-id="64133-113">У спливаючому меню **відомості** натисніть кнопку **додаткові відомості**.</span><span class="sxs-lookup"><span data-stu-id="64133-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="64133-114">Слід звернути увагу на відомості кожного запису аудиту, щоб визначити, чи справа пов'язана з пересиланнею електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="64133-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="64133-115">**Об'єктиідентифікатор**: псевдонім значення поштової скриньки, який було змінено.</span><span class="sxs-lookup"><span data-stu-id="64133-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="64133-116">**Параметри**: _переадресації_ вказують на цільову адресу електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="64133-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="64133-117">**Userid**: користувач, який налаштував пересилання електронної пошти на поштову скриньку, у полі **ідентифікатор об'єкта** .</span><span class="sxs-lookup"><span data-stu-id="64133-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="64133-118">Для отримання додаткових відомостей див. [визначення, які встановлюють пересилання електронної пошти для поштової скриньки](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span><span class="sxs-lookup"><span data-stu-id="64133-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
