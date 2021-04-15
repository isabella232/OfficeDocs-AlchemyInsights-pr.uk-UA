---
title: Помилка. Правила на цьому комп'ютері не збігаються
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782973"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="68302-102">Помилка. Правила на цьому комп'ютері не збігаються</span><span class="sxs-lookup"><span data-stu-id="68302-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="68302-103">Відомості про те, як переглянути оновлений стан відомої проблеми, див. в статті Правила на цьому комп'ютері не відповідають [правилам на сервері Microsoft Exchange.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="68302-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="68302-104">Команда Outlook впроваджує виправлення в збірці 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="68302-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="68302-105">Виправлення вже доступне в програмі оцінювачів із ралі та перейде до щомісячного каналу оновлення наприкінці червня 2020 р.</span><span class="sxs-lookup"><span data-stu-id="68302-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="68302-106">Коли ви вкажете фіксовану збірку, може з'явитися повідомлення "Які правила слід зберігати" один раз востаннє.</span><span class="sxs-lookup"><span data-stu-id="68302-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="68302-107">Коли з'явиться відповідний запит, виберіть Сервер, а потім поверніться до програми Outlook і знову ввімкніть усі вимкнуті правила.</span><span class="sxs-lookup"><span data-stu-id="68302-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="68302-108">Доки виправлення не з'явиться, скористайтеся наведеним нижче способом вирішення.</span><span class="sxs-lookup"><span data-stu-id="68302-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="68302-109">**Спосіб вирішення. В останніх** звітах ця проблема виникла лише в класичній програмі Outlook.</span><span class="sxs-lookup"><span data-stu-id="68302-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="68302-110">Якщо проблема не зникає, ми редагуйте їх, а потім створюйте та редагуйте правила лише у веб-програмі OWA (Outlook Web App), доки проблему не буде вирішено.</span><span class="sxs-lookup"><span data-stu-id="68302-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="68302-111">Якщо ви не можете видалити правила вручну, ви можете виконати команду Outlook під час запуску програми Outlook, запустивши Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="68302-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="68302-112">При цьому буде видалено правила клієнта та сервера.</span><span class="sxs-lookup"><span data-stu-id="68302-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="68302-113">Усі правила для всіх облікових записів у профілі Outlook буде видалено.</span><span class="sxs-lookup"><span data-stu-id="68302-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="68302-114">Цю команду додатково описано в статті Перемикачі командного рядка.</span><span class="sxs-lookup"><span data-stu-id="68302-114">This command is further documented in the Command-line switches article.</span></span>

