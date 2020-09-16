---
title: Виправлення неполадок із електронною поштою
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658755"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="82cdd-102">Виправлення неполадок із електронною поштою</span><span class="sxs-lookup"><span data-stu-id="82cdd-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="82cdd-103">Перевірка функції для поштової скриньки: \*\*Get-EventsFromEmailConfiguration-Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="82cdd-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="82cdd-104">Після цього перейдіть на вкладку "події з електронної пошти", що **експортується – MailboxDiagnosticLogs <mailbox> -компонент "хронопрофіль** "</span><span class="sxs-lookup"><span data-stu-id="82cdd-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="82cdd-105">У журналах "події з електронної пошти" Дізнайтеся, що відповідає елементу в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="82cdd-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="82cdd-106">"Довірчого значення" визначає, чи додано елемент або ні.</span><span class="sxs-lookup"><span data-stu-id="82cdd-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="82cdd-107">Події буде додано лише за умови, що довірчі = "надійні".</span><span class="sxs-lookup"><span data-stu-id="82cdd-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="82cdd-108">Показник Truecscore визначається за властивостями SPF, DKIM або DKIM, які знаходяться в заголовку повідомлення.</span><span class="sxs-lookup"><span data-stu-id="82cdd-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="82cdd-109">Щоб переглянути ці властивості, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="82cdd-109">To view these properties:</span></span>

<span data-ttu-id="82cdd-110">**Робочий стіл Outlook**</span><span class="sxs-lookup"><span data-stu-id="82cdd-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="82cdd-111">Відкриття елемента</span><span class="sxs-lookup"><span data-stu-id="82cdd-111">Open the item</span></span>
- <span data-ttu-id="82cdd-112">Властивості файлу > – > заголовки Інтернету</span><span class="sxs-lookup"><span data-stu-id="82cdd-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="82cdd-113">або</span><span class="sxs-lookup"><span data-stu-id="82cdd-113">or</span></span>

<span data-ttu-id="82cdd-114">**Mffmapi**</span><span class="sxs-lookup"><span data-stu-id="82cdd-114">**MFCMapi**</span></span>

- <span data-ttu-id="82cdd-115">Перехід до елемента в папці "Вхідні"</span><span class="sxs-lookup"><span data-stu-id="82cdd-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="82cdd-116">Пошук PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="82cdd-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="82cdd-117">Ці властивості визначаються та записуються під час транспортування та маршрутизації.</span><span class="sxs-lookup"><span data-stu-id="82cdd-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="82cdd-118">Щоб отримати додаткові виправлення неполадок, можливо, знадобиться стежити за допомогою транспортної підтримки про помилки в SPF, DKIM і. або DKIM.</span><span class="sxs-lookup"><span data-stu-id="82cdd-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>