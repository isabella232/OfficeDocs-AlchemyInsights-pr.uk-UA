---
title: Усунення несправностей подій з електронної пошти
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569399"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="c9c9f-102">Усунення несправностей подій з електронної пошти</span><span class="sxs-lookup"><span data-stu-id="c9c9f-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="c9c9f-103">Перевірте, чи ввімкнуто функцію для поштової скриньки: \*\*Get-подія Sfromemailconfiguration-посвідчення <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="c9c9f-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="c9c9f-104">Потім подивіться на "події з електронної пошти" журнали **експорт-MailboxDiagnosticLogs <mailbox> -компонент timeprofile**</span><span class="sxs-lookup"><span data-stu-id="c9c9f-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="c9c9f-105">У журналах "події з електронної пошти" знайдіть пункт Інтернетаповідомлення, яке відповідає елементу в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="c9c9f-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="c9c9f-106">Довірчого оцінка визначає, чи елемент додано чи ні.</span><span class="sxs-lookup"><span data-stu-id="c9c9f-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="c9c9f-107">Події будуть додаватися, лише якщо довірчого показника = "довірений".</span><span class="sxs-lookup"><span data-stu-id="c9c9f-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="c9c9f-108">Довірчого оцінки визначається SPF, DKIM або DKIM властивості, які в заголовку повідомлення.</span><span class="sxs-lookup"><span data-stu-id="c9c9f-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="c9c9f-109">Щоб переглянути ці властивості:</span><span class="sxs-lookup"><span data-stu-id="c9c9f-109">To view these properties:</span></span>

<span data-ttu-id="c9c9f-110">**Desktop Outlook**</span><span class="sxs-lookup"><span data-stu-id="c9c9f-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="c9c9f-111">Відкрити елемент</span><span class="sxs-lookup"><span data-stu-id="c9c9f-111">Open the item</span></span>
- <span data-ttu-id="c9c9f-112">Файл-> властивості-> Інтернет-заголовки</span><span class="sxs-lookup"><span data-stu-id="c9c9f-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="c9c9f-113">Або</span><span class="sxs-lookup"><span data-stu-id="c9c9f-113">or</span></span>

<span data-ttu-id="c9c9f-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="c9c9f-114">**MFCMapi**</span></span>

- <span data-ttu-id="c9c9f-115">Перехід до елемента в папці «Вхідні»</span><span class="sxs-lookup"><span data-stu-id="c9c9f-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="c9c9f-116">Шукайте PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="c9c9f-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="c9c9f-117">Ці властивості визначаються і записуються під час транспортування та маршрутизації.</span><span class="sxs-lookup"><span data-stu-id="c9c9f-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="c9c9f-118">Щоб отримати додаткові відомості про виправлення неполадок, можливо, потрібно буде виконати транспортні підтримки про збої в SPF, DKIM та. or DKIM.</span><span class="sxs-lookup"><span data-stu-id="c9c9f-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>