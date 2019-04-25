---
title: 1332 OWA - вхідні правила не виконуєте для поштової скриньки
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372581"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="9af18-102">Вхідні правило не працює належним чином</span><span class="sxs-lookup"><span data-stu-id="9af18-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="9af18-103">Підтвердження таких настройок:</span><span class="sxs-lookup"><span data-stu-id="9af18-103">Verify the following settings:</span></span>

- <span data-ttu-id="9af18-104">Можна переспрямувати повідомлення, пересиланню чи була надіслана відповідь, автоматично заснований на правилах вхідної тільки один раз.</span><span class="sxs-lookup"><span data-stu-id="9af18-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="9af18-105">Переспрямування правило (правило для вхідних повідомлень або правило потік пошти, також відомі як правила транспортування) можна додати максимум десять пересилання одержувачам повідомлення.</span><span class="sxs-lookup"><span data-stu-id="9af18-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="9af18-106">Докладніше перегляньте [журнал, транспорту і «вхідні» правилом меж](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="9af18-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="9af18-107">Правила для папки «Вхідні» не працюють на поштову скриньку альтернативний журналів.</span><span class="sxs-lookup"><span data-stu-id="9af18-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="9af18-108">Докладніше про поштової скриньки протоколювання альтернативний побачити [Альтернативний журнальної поштової скриньки](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="9af18-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="9af18-109">Для усунення цих проблем, побачити [2829319 КБ](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="9af18-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="9af18-110">Якщо не застосовувати попередніх випусків, запустити папки «Вхідні» правилом діагностичний звіт перед ескалації питання до служби підтримки Microsoft:</span><span class="sxs-lookup"><span data-stu-id="9af18-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="9af18-111">Відкриття поштової скриньки в Outlook в Інтернеті та кнопку **Параметри** \> **Параметри** \> **упорядкувати електронну** \> **Вхідні правила**.</span><span class="sxs-lookup"><span data-stu-id="9af18-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="9af18-112">У нижній частині сторінки натисніть, **Якщо правила не працюють натисніть тут, щоб створити діагностичний звіт**.</span><span class="sxs-lookup"><span data-stu-id="9af18-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
