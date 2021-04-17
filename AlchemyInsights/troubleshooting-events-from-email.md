---
title: Виправлення неполадок, пов'язаних із подіями з електронної пошти
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834860"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="87346-102">Виправлення неполадок, пов'язаних із подіями з електронної пошти</span><span class="sxs-lookup"><span data-stu-id="87346-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="87346-103">Перевірка активації функції для поштової скриньки: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="87346-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="87346-104">Потім перегляньте журнали "Події з електронної пошти" **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="87346-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="87346-105">У журналах "Події з електронної пошти" знайдіть елемент InternetMessageId, який збігається з елементом у поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="87346-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="87346-106">Параметр TrustScore визначає, чи додається елемент.</span><span class="sxs-lookup"><span data-stu-id="87346-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="87346-107">Події додаються, лише якщо значення TrustScore = "Trusted" (Довіряти).</span><span class="sxs-lookup"><span data-stu-id="87346-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="87346-108">Значення TrustScore визначається властивостями SPF, Dkim або Dmarc у заголовку повідомлення.</span><span class="sxs-lookup"><span data-stu-id="87346-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="87346-109">Щоб переглянути ці властивості, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="87346-109">To view these properties:</span></span>

<span data-ttu-id="87346-110">**Класична програма Outlook**</span><span class="sxs-lookup"><span data-stu-id="87346-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="87346-111">Відкриття елемента</span><span class="sxs-lookup"><span data-stu-id="87346-111">Open the item</span></span>
- <span data-ttu-id="87346-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="87346-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="87346-113">або</span><span class="sxs-lookup"><span data-stu-id="87346-113">or</span></span>

<span data-ttu-id="87346-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="87346-114">**MFCMapi**</span></span>

- <span data-ttu-id="87346-115">Перехід до елемента в папці "Вхідні"</span><span class="sxs-lookup"><span data-stu-id="87346-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="87346-116">Знайдіть PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="87346-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="87346-117">Ці властивості визначаються та записуються під час транспортування та маршрутизації.</span><span class="sxs-lookup"><span data-stu-id="87346-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="87346-118">Щоб додатково виправити неполадки, може знадобитися виконати вказівки зі служби підтримки транспортування, пов'язаної з помилками SPF, DKIM і DMARC.</span><span class="sxs-lookup"><span data-stu-id="87346-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>