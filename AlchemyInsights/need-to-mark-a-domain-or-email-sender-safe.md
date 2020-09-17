---
title: Потрібно, щоб можна було відмітити домен або відправника електронної пошти в безпеці?
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803266"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="d5698-102">Потрібно, щоб можна було відмітити домен або відправника електронної пошти в безпеці?</span><span class="sxs-lookup"><span data-stu-id="d5698-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="d5698-103">**Не рекомендується використовувати списки надійних відправників** , оскільки вона відкриває свою організацію в спам, phish та спуфінгу.</span><span class="sxs-lookup"><span data-stu-id="d5698-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="d5698-104">Однак, якщо є потреба в бізнесі, **радимо** використовувати **[правила передавання пошти](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="d5698-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="d5698-105">Наше керівництво забезпечує автентифікацію відправника (перевіряє, чи не підроблений домен).</span><span class="sxs-lookup"><span data-stu-id="d5698-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="d5698-106">**Примітка**. не радимо керувати хибними спрацьовуванням за допомогою списків надійних відправників, оскільки винятки з фільтрування спаму можуть відкрити свою організацію для атак з безпеки.</span><span class="sxs-lookup"><span data-stu-id="d5698-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="d5698-107">Якщо ваші повідомлення неправильно позначені як спам або Небажана пошта, **[повідомте про це повідомлення та файли до корпорації Майкрософт](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="d5698-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="d5698-108">Надійні відправники в Outlook, дозволені список відправників або список дозволених доменів у політиці захисту від спаму **слід уникати** , тому що відправники оминають всі функції спаму, пародія та флеш-захист, а також автентифікацію ВІДПРАВНИКА (SPF, DKIM, DKIM).</span><span class="sxs-lookup"><span data-stu-id="d5698-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="d5698-109">Цей метод можна використовувати лише для тимчасового тестування.</span><span class="sxs-lookup"><span data-stu-id="d5698-109">This method is best used for temporary testing only.</span></span>
