---
title: Надсилання вихідної пошти до папки небажаної пошти
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
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769204"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="3560c-102">Надсилання вихідної пошти до папки небажаної пошти</span><span class="sxs-lookup"><span data-stu-id="3560c-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="3560c-103">Якщо ви бачите вихідні повідомлення, позначені як небажані, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="3560c-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="3560c-104">Якщо ви ще не зробили цього, спробуйте [налаштувати сповіщення про політику вихідної небажаної пошти](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="3560c-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="3560c-105">Використовуйте [трасування повідомлень](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) , щоб дізнатися, чи вихідне повідомлення містить **спам** -значення події з додатковою деталізацією: **використання високого ризику в пулі**.</span><span class="sxs-lookup"><span data-stu-id="3560c-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="3560c-106">Для цих повідомлень перевірте вміст повідомлення, щоб дізнатися, що може вважатися спамом.</span><span class="sxs-lookup"><span data-stu-id="3560c-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="3560c-107">Наприклад, підписи можуть інколи спричиняти проблеми для багатьох користувачів.</span><span class="sxs-lookup"><span data-stu-id="3560c-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="3560c-108">Якщо у вас кілька прикладів надійних вихідних повідомлень, які позначено як небажані, відкрийте квиток підтримки та попросіть агента підтримки надіслати повідомлення як помилкові позитивні результати для наших аналітиків спаму.</span><span class="sxs-lookup"><span data-stu-id="3560c-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="3560c-109">Будьте готові надати зразок повідомлень, які містять усі заголовки повідомлень.</span><span class="sxs-lookup"><span data-stu-id="3560c-109">Be prepared to provide sample messages that include all message headers.</span></span>
