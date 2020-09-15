---
title: 1332 OWA-вхідні не виконують правила для поштової скриньки
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721612"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="c6eda-102">Правило для папки "Вхідні" не працює належним чином</span><span class="sxs-lookup"><span data-stu-id="c6eda-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="c6eda-103">Перевірте наведені нижче настройки в Інтернет-версії Outlook.</span><span class="sxs-lookup"><span data-stu-id="c6eda-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="c6eda-104">Повідомлення можна перенаправлятися, пересилати або відповідати автоматично на основі правил для папки "Вхідні" лише один раз.</span><span class="sxs-lookup"><span data-stu-id="c6eda-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="c6eda-105">Правило переспрямування (правило для папки "Вхідні" або "потік пошти", також відомий як правило транспортування) може додавати до повідомлення максимум десяти одержувачів пересилання.</span><span class="sxs-lookup"><span data-stu-id="c6eda-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="c6eda-106">Докладні відомості наведено в статті [обмеження правил для журналу, транспорту та папки "Вхідні"](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="c6eda-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="c6eda-107">Правила для папки "Вхідні" не працюють в альтернативному поштовій скриньці журналювання.</span><span class="sxs-lookup"><span data-stu-id="c6eda-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="c6eda-108">Докладні відомості про альтернативну поштову скриньку журналювання наведено в статті [Альтернативна поштова скринька журналів](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c6eda-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="c6eda-109">Щоб вирішити ці проблеми, ознайомтеся з пунктом [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="c6eda-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="c6eda-110">Якщо попередні проблеми не застосовуватимуться, запустіть звіт про діагностику правил для папки "Вхідні", перш ніж перерости цю проблему до служби підтримки Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c6eda-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="c6eda-111">Відкрийте поштову скриньку в Інтернет-версії Outlook і натисніть кнопку</span><span class="sxs-lookup"><span data-stu-id="c6eda-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="c6eda-112">**Параметри**  >  **Переглянути всі настройки Outlook**  >  **Пошта**  >  **Правила**.</span><span class="sxs-lookup"><span data-stu-id="c6eda-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="c6eda-113">У нижній частині сторінки клацніть, **Якщо правила не працюють, натисніть тут, щоб створити діагностичний звіт**.</span><span class="sxs-lookup"><span data-stu-id="c6eda-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
