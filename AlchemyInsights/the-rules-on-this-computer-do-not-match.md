---
title: "Помилка: правила на цьому комп'ютері не збігаються"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664267"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="0e8b7-102">Помилка: правила на цьому комп'ютері не збігаються</span><span class="sxs-lookup"><span data-stu-id="0e8b7-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="0e8b7-103">Щоб переглянути оновлений стан цієї відомої проблеми, див. [правила на цьому комп'ютері не відповідають правилам Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="0e8b7-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="0e8b7-104">Команда Outlook реалізувала виправити в Build 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="0e8b7-105">Виправити вже на Insider швидко і піде на щомісячний канал в кінці червня 2020.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="0e8b7-106">Після того, як ви фіксованого побудувати ви можете отримати підказку "які правила ви хочете зберегти" в останній раз.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="0e8b7-107">Виберіть сервер, коли з'явиться запит, а потім поверніться в Outlook і знову ввімкніть будь-які правила, які були вимкнені.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="0e8b7-108">До Виправлення доступне, будь ласка, використовуйте такий спосіб:</span><span class="sxs-lookup"><span data-stu-id="0e8b7-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="0e8b7-109">**Тимчасове рішення**: у останніх звітах виникла проблема для тих, які мають лише створені клієнтські правила в Outlook Desktop.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="0e8b7-110">Якщо ви продовжуєте працювати з цією проблемою, спробуйте видалити правила, а потім створити та редагувати правила лише в OWA (веб-застосунок Outlook Web App), доки проблему не буде усунуто.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="0e8b7-111">Якщо ви не можете видалити правила вручну, ви можете запустити команду Outlook під час запуску Outlook, запустивши Outlook. exe/чищення.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="0e8b7-112">Це видалить правила клієнта та сервера.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="0e8b7-113">Він видалить Усі правила для всіх облікових записів у профілі Outlook.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="0e8b7-114">Ця команда, Далі описано у статті командного рядка, перемикачі.</span><span class="sxs-lookup"><span data-stu-id="0e8b7-114">This command is further documented in the Command-line switches article.</span></span>

