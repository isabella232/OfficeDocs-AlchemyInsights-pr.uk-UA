---
title: "Помилка: правила на цьому комп'ютері не збігаються"
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690984"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="57617-102">Помилка: правила на цьому комп'ютері не збігаються</span><span class="sxs-lookup"><span data-stu-id="57617-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="57617-103">Щоб переглянути оновлений стан цієї відомої проблеми, ознайомтеся з [правилами на цьому комп'ютері, які не відповідають правилам в Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="57617-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="57617-104">Команда Outlook реалізувала виправлення в збірці 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="57617-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="57617-105">Виправлення вже на рівні інсайдерів і буде Перемотка на щомісячний канал наприкінці червня 2020.</span><span class="sxs-lookup"><span data-stu-id="57617-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="57617-106">Після встановлення фіксованого складання ви можете отримати підказку "правила, які потрібно зберегти" в останній раз.</span><span class="sxs-lookup"><span data-stu-id="57617-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="57617-107">Виберіть сервер, коли з'явиться відповідний запит, і поверніться до програми Outlook і повторно ввімкніть всі правила, які було вимкнуто.</span><span class="sxs-lookup"><span data-stu-id="57617-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="57617-108">Доки виправлення не буде доступно, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="57617-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="57617-109">**Спосіб вирішення**: у недавніх звітах виникла проблема для тих, хто створив лише правила клієнта в програмі Outlook для настільних комп'ютерів.</span><span class="sxs-lookup"><span data-stu-id="57617-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="57617-110">Якщо ви продовжуватимете працювати з цією проблемою, радимо видалити правила, а потім створювати й редагувати правила лише в розділі OWA (веб-застосунок Outlook Web App), доки проблему не вирішено.</span><span class="sxs-lookup"><span data-stu-id="57617-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="57617-111">Якщо ви не можете видалити правила вручну, під час запуску програми Outlook можна запустити команду Outlook, запустивши Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="57617-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="57617-112">Після цього буде видалено правила клієнта та сервера.</span><span class="sxs-lookup"><span data-stu-id="57617-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="57617-113">Буде видалено всі правила для всіх облікових записів у профілі Outlook.</span><span class="sxs-lookup"><span data-stu-id="57617-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="57617-114">Ця команда ще більше документована в статті Перемикачі командного рядка.</span><span class="sxs-lookup"><span data-stu-id="57617-114">This command is further documented in the Command-line switches article.</span></span>

