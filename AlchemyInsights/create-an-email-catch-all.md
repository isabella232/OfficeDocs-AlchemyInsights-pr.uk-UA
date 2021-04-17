---
title: Створення повідомлення електронної пошти для всіх
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816221"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="d0746-102">Створення повідомлення електронної пошти для всіх</span><span class="sxs-lookup"><span data-stu-id="d0746-102">Create an email catch all</span></span>

<span data-ttu-id="d0746-103">Використання уловів наполегливо загромаджується.</span><span class="sxs-lookup"><span data-stu-id="d0746-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="d0746-104">Краще повернути відправника звіт про те, що його повідомлення не вдалося доставити за адресою, щоб вони могли вживати певних заходів.</span><span class="sxs-lookup"><span data-stu-id="d0746-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="d0746-105">Крім того, ви можете обмежити відстежування поштової скриньки лише припустимими адресами електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="d0746-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="d0746-106">Усі поштові скриньки отримають багато спаму та, врешті-решт, можуть заповнюватися, якщо ви не стежите за ним.</span><span class="sxs-lookup"><span data-stu-id="d0746-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="d0746-107">(Є обмеження для отримання).)</span><span class="sxs-lookup"><span data-stu-id="d0746-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="d0746-108">Якщо ви вирішите продовжити, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="d0746-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="d0746-109">Створіть динамічну групу розсилки & "Усі типи одержувачів".</span><span class="sxs-lookup"><span data-stu-id="d0746-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="d0746-110">Створіть спеціальну поштову скриньку, щоб зацікавити електронні листи, наприклад catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="d0746-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="d0746-111">Для певного домену встановіть для параметра DomainType значення InternalRelay (Внутрішній домен).</span><span class="sxs-lookup"><span data-stu-id="d0746-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="d0746-112">Якщо згодом ви вилучите всі ці відомості, обов'язково поверніть домен до значення Повноваження.</span><span class="sxs-lookup"><span data-stu-id="d0746-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="d0746-113">Створіть правило транспортування пошти таким чином:</span><span class="sxs-lookup"><span data-stu-id="d0746-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="d0746-114">Відправник має значення "За межами організації"</span><span class="sxs-lookup"><span data-stu-id="d0746-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="d0746-115">Переспрямування повідомлення на Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="d0746-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="d0746-116">За винятком, коли одержувач є учасником групи allusers@domain.com (група розсилки містить усіх учасників)</span><span class="sxs-lookup"><span data-stu-id="d0746-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="d0746-117">Перевірка додавання нових поштових скриньок до динамічної групи розсилки</span><span class="sxs-lookup"><span data-stu-id="d0746-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
