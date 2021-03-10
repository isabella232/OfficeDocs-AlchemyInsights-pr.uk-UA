---
title: Виправлення параметрів політики та поштової скриньки користувача
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695897"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="d04c4-102">Виправлення параметрів політики та поштової скриньки користувача</span><span class="sxs-lookup"><span data-stu-id="d04c4-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="d04c4-103">Це повідомлення вплине на настройки небажаної пошти в поштовій скриньці.</span><span class="sxs-lookup"><span data-stu-id="d04c4-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="d04c4-104">Щоб переглянути настройки, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="d04c4-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="d04c4-105">Запуск оболонки керування Exchange.</span><span class="sxs-lookup"><span data-stu-id="d04c4-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="d04c4-106">Докладні відомості наведено в статті [відкриття оболонки керування Exchange](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="d04c4-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="d04c4-107">Виконати цю команду (за допомогою адреси електронної пошти користувача):  **Get-mailboxjunkmailconfiguration-Identity "User@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="d04c4-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="d04c4-108">Перевірте, чи є адреса електронної пошти відправника, що входить до складу **Trusedsendersanddomains** або **blockkedsendersanddomains**.</span><span class="sxs-lookup"><span data-stu-id="d04c4-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="d04c4-109">Якщо адреса електронної пошти міститься в одному з списків, можливо, доведеться видалити його.</span><span class="sxs-lookup"><span data-stu-id="d04c4-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="d04c4-110">Докладні відомості можна знайти в статті " [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)".</span><span class="sxs-lookup"><span data-stu-id="d04c4-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
