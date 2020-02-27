---
title: Створити лист зловити все
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286312"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="da3ff-102">Створити лист зловити все</span><span class="sxs-lookup"><span data-stu-id="da3ff-102">Create an email catch all</span></span>

<span data-ttu-id="da3ff-103">Використання зловити все це настійно рекомендується.</span><span class="sxs-lookup"><span data-stu-id="da3ff-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="da3ff-104">Краще забезпечити повернення до відправника, даючи відправникам знати їхнє повідомлення не може бути доставлений як адресована, щоб вони могли вжити заходів.</span><span class="sxs-lookup"><span data-stu-id="da3ff-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="da3ff-105">Ви також можете обмежити відстежуваний поштову скриньку лише зловити раніше дійсні адреси електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="da3ff-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="da3ff-106">Будь-який зловити всі поштової скриньки буде отримувати багато спаму і може в кінцевому підсумку заповнити, якщо не уважно контролюватися.</span><span class="sxs-lookup"><span data-stu-id="da3ff-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="da3ff-107">(Є отримання лімітів.)</span><span class="sxs-lookup"><span data-stu-id="da3ff-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="da3ff-108">Якщо ви вирішите продовжити, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="da3ff-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="da3ff-109">Створення динамічної групи розсилки & включати "Усі типи одержувачів".</span><span class="sxs-lookup"><span data-stu-id="da3ff-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="da3ff-110">Створіть спеціальну поштову скриньку, щоб зловити електронні листи, наприклад catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="da3ff-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="da3ff-111">Для певного домену встановіть тип домену на "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="da3ff-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="da3ff-112">Якщо пізніше видалити зловити все, не забудьте встановити домен назад в авторитетне.</span><span class="sxs-lookup"><span data-stu-id="da3ff-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="da3ff-113">Створіть правило транспортування Mailflow таким чином:</span><span class="sxs-lookup"><span data-stu-id="da3ff-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="da3ff-114">Якщо відправник "поза організацією"</span><span class="sxs-lookup"><span data-stu-id="da3ff-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="da3ff-115">Перенаправити повідомлення до Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="da3ff-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="da3ff-116">За винятком випадків, коли одержувач є членом allusers@domain.com (група розсилки містить всі члени)</span><span class="sxs-lookup"><span data-stu-id="da3ff-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="da3ff-117">Перевірте, чи додаються нові поштові скриньки до динамічної групи розсилки</span><span class="sxs-lookup"><span data-stu-id="da3ff-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
