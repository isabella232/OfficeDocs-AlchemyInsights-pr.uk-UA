---
title: Вирішення проблем з автентифікацією SMTP
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
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826436"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="2fbad-102">Вирішення проблем з автентифікацією SMTP</span><span class="sxs-lookup"><span data-stu-id="2fbad-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="2fbad-103">Якщо під час спроби надіслати повідомлення електронної пошти SMTP з'являється помилка 5.7.57 або 5.7.3 та автентифікація за допомогою клієнта або програми, перевірте таке:</span><span class="sxs-lookup"><span data-stu-id="2fbad-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="2fbad-104">Автентифікований надсилання SMTP може бути вимкнуто в клієнта або в поштовій скриньці, яку ви намагаєтеся використати (перевірте обидва параметри).</span><span class="sxs-lookup"><span data-stu-id="2fbad-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="2fbad-105">Докладні відомості див. в статтях Увімкнення та вимкнення надсилання [SMTP-повідомлень автентифікованого клієнта.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="2fbad-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="2fbad-106">Перевірте, [чи ввімкнуто](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) за замовчуванням azure Security Defaults для вашого клієнта. Якщо цей параметр увімкнуто, помилка під час автентифікації SMTP за допомогою базової автентифікації (так званої застарілої) не вдасться.</span><span class="sxs-lookup"><span data-stu-id="2fbad-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
