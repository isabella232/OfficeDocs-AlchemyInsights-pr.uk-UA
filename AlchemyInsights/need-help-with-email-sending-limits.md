---
title: Потрібна допомога в електронній пошті обмеження відправки?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/20/2020
ms.locfileid: "44358362"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="c4a29-102">Потрібна допомога в електронній пошті обмеження відправки?</span><span class="sxs-lookup"><span data-stu-id="c4a29-102">Need help with email sending limits?</span></span>

<span data-ttu-id="c4a29-103">Нижче знаходиться **по-дизайн відправки лімітів** , що застосовуються в сервісі.</span><span class="sxs-lookup"><span data-stu-id="c4a29-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="c4a29-104">Більш детальну інформацію про ці обмеження описано [тут](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="c4a29-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="c4a29-105">Для запобігання доставки небажаних масових повідомлень, ми застосовуємо для кожного користувача **обмеження частоти для всіх вихідних і внутрішніх повідомлень**.</span><span class="sxs-lookup"><span data-stu-id="c4a29-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="c4a29-106">У всіх SKUs це обмеження **10 000 одержувачів на день**.</span><span class="sxs-lookup"><span data-stu-id="c4a29-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="c4a29-107">Клієнти, яким потрібно надсилати легальний обсяг комерційної електронної пошти (наприклад, інформаційні бюлетені для клієнтів), повинні використовувати сторонні постачальники, які спеціалізуються на цих службах.</span><span class="sxs-lookup"><span data-stu-id="c4a29-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="c4a29-108">**Примітка**: після того, як обмеження частоти одержувачів досягнуто, повідомлення не надсилатимуться з поштової скриньки, доки кількість одержувачів, які було надіслано повідомлення за останні 24 годин, опускається нижче межі.</span><span class="sxs-lookup"><span data-stu-id="c4a29-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="c4a29-109">Користувач не зможе надсилати повідомлення до цього моменту.</span><span class="sxs-lookup"><span data-stu-id="c4a29-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="c4a29-110">Обмеження швидкості повідомлення **30 повідомлень на хвилину** застосовується по всіх skus.</span><span class="sxs-lookup"><span data-stu-id="c4a29-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="c4a29-111">Це визначає, скільки повідомлень користувач може надсилати зі свого облікового запису Exchange Online протягом указаного періоду.</span><span class="sxs-lookup"><span data-stu-id="c4a29-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="c4a29-112">**Максимальна кількість одержувачів, дозволених у полях Кому, копія та Прихована копія** для окремого повідомлення електронної пошти, у всіх skus, є **1000 одержувачів**.</span><span class="sxs-lookup"><span data-stu-id="c4a29-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="c4a29-113">Щоб налаштувати цю межу, перейдіть [сюди](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="c4a29-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
