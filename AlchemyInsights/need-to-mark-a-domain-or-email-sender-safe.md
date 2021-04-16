---
title: Потрібно позначити домен або відправника електронної пошти як надійний?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792153"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="2fe8f-102">Потрібно позначити домен або відправника електронної пошти як надійний?</span><span class="sxs-lookup"><span data-stu-id="2fe8f-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="2fe8f-103">Ми не **рекомендуємо** використовувати списки надійних відправників, оскільки він відкриває організацію для спаму, фішингових і спуфінгових атак.</span><span class="sxs-lookup"><span data-stu-id="2fe8f-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="2fe8f-104">Проте якщо вимоги компанії висувають певні вимоги, для цього радимо **[використовувати](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** правила потоків пошти. </span><span class="sxs-lookup"><span data-stu-id="2fe8f-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="2fe8f-105">Наші указівки гарантують, що автентифікація відправника (перевіряє, що домен надсилання не спуфінгується).</span><span class="sxs-lookup"><span data-stu-id="2fe8f-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="2fe8f-106">**Примітка.** Ми не радимо виправляти хибні результати за допомогою списків надійних відправників, оскільки винятки з фільтрування спаму можуть відкрити організацію в атаках безпеки.</span><span class="sxs-lookup"><span data-stu-id="2fe8f-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="2fe8f-107">Якщо ваші користувачів отримують повідомлення, помічені як спам або небажана пошта, повідомте про повідомлення та файли до **[корпорації Майкрософт.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="2fe8f-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="2fe8f-108">Надійні відправники в Outlook, список дозволених відправників або  список дозволених доменів у політиках захисту від спаму слід уникати, оскільки відправники не можуть обійти всі спам, спуфінг і фіш-захист і автентифікацію відправника (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="2fe8f-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="2fe8f-109">Цей метод краще використовувати лише для тимчасового тестування.</span><span class="sxs-lookup"><span data-stu-id="2fe8f-109">This method is best used for temporary testing only.</span></span>
