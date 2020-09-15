---
title: Створення повідомлення електронної пошти "спіймати все"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713007"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="31b6c-102">Створення повідомлення електронної пошти "спіймати все"</span><span class="sxs-lookup"><span data-stu-id="31b6c-102">Create an email catch all</span></span>

<span data-ttu-id="31b6c-103">Використання спіймати все сильно не рекомендується.</span><span class="sxs-lookup"><span data-stu-id="31b6c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="31b6c-104">Щоб відправник не міг отримувати повідомлення про те, що його не можна було доставити, то краще надати відправнику відомості про те, що вони можуть виконувати дії.</span><span class="sxs-lookup"><span data-stu-id="31b6c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="31b6c-105">Ви також можете обмежити відповідну поштову скриньку, щоб зловити раніше дійсні адреси електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="31b6c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="31b6c-106">Усі поштові скриньки можуть отримувати багато спаму, а потім заповнювати їх, якщо вони не будуть ретельно контролюватися.</span><span class="sxs-lookup"><span data-stu-id="31b6c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="31b6c-107">(Є обмеження на отримання.)</span><span class="sxs-lookup"><span data-stu-id="31b6c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="31b6c-108">Якщо ви вирішите продовжити, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="31b6c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="31b6c-109">Створення динамічної групи розсилки & містять "Усі типи одержувачів".</span><span class="sxs-lookup"><span data-stu-id="31b6c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="31b6c-110">Створюйте спеціальні поштові скриньки, щоб спіймати повідомлення електронної пошти, наприклад catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="31b6c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="31b6c-111">Для певного домену настройте тип домену на "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="31b6c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="31b6c-112">Якщо ви згодом видалите всі елементи "спіймати все", переконайтеся, що домен повернутися до авторитетного значення.</span><span class="sxs-lookup"><span data-stu-id="31b6c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="31b6c-113">Створення правила транспортування поштової потоки таким, як описано нижче.</span><span class="sxs-lookup"><span data-stu-id="31b6c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="31b6c-114">Якщо відправник – "поза організацією"</span><span class="sxs-lookup"><span data-stu-id="31b6c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="31b6c-115">Переспрямування повідомлення до Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="31b6c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="31b6c-116">За винятком випадків, коли одержувач входить до складу allusers@domain.com (група розсилки містить всі учасники)</span><span class="sxs-lookup"><span data-stu-id="31b6c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="31b6c-117">Перевірка того, що нові поштові скриньки додаються до динамічної групи розсилки</span><span class="sxs-lookup"><span data-stu-id="31b6c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
