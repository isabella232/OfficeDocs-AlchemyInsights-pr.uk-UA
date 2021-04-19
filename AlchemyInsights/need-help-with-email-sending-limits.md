---
title: Потрібна довідка з обмежень для надсилання електронних листів?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836300"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="db14f-102">Потрібна довідка з обмежень для надсилання електронних листів?</span><span class="sxs-lookup"><span data-stu-id="db14f-102">Need help with email sending limits?</span></span>

<span data-ttu-id="db14f-103">Нижче наведено **поетапні обмеження,** які застосовуються для надсилання повідомлень у службі.</span><span class="sxs-lookup"><span data-stu-id="db14f-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="db14f-104">Докладні відомості про ці обмеження див. [тут.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)</span><span class="sxs-lookup"><span data-stu-id="db14f-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="db14f-105">Щоб обмежити доставку незапитаних групових повідомлень, до всіх вихідних і внутрішніх повідомлень застосовуються обмеження частоти надсилання **повідомлень кожного користувача.**</span><span class="sxs-lookup"><span data-stu-id="db14f-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="db14f-106">У всіх облікових номерах це обмеження до **10 000 одержувачів на день.**</span><span class="sxs-lookup"><span data-stu-id="db14f-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="db14f-107">Клієнти, яким потрібно надіслати надійну групову комерційну електронну пошту (наприклад, бюлетень клієнтів), мають використовувати сторонніх постачальників, які спеціалізуються на цих службах.</span><span class="sxs-lookup"><span data-stu-id="db14f-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="db14f-108">**Примітка.** Після досягнення обмеження частоти надсилання повідомлень із поштової скриньки не можна надсилати до кількості одержувачів, які надсилали повідомлення за останні 24 години нижче обмеження.</span><span class="sxs-lookup"><span data-stu-id="db14f-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="db14f-109">Користувач не зможе надсилати повідомлення до цього моменту.</span><span class="sxs-lookup"><span data-stu-id="db14f-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="db14f-110">У всіх облікових **номерах застосовується обмеження 30** повідомлень за хвилину.</span><span class="sxs-lookup"><span data-stu-id="db14f-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="db14f-111">Це визначає, скільки повідомлень користувач може надсилати з облікового запису Exchange Online протягом певного періоду.</span><span class="sxs-lookup"><span data-stu-id="db14f-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="db14f-112">Максимальна **кількість** одержувачів, дозволених у полях "Обов'язковий", "Копія" та "ПК" для одного повідомлення електронної пошти в усіх облікових номерах, – **1000 одержувачів.**</span><span class="sxs-lookup"><span data-stu-id="db14f-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="db14f-113">Щоб налаштувати це обмеження, перейдіть [сюди.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)</span><span class="sxs-lookup"><span data-stu-id="db14f-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
