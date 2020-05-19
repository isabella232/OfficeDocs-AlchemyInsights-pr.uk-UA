---
title: Потрібно позначити домен або відправника електронної пошти безпечним?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281240"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="c72b5-102">Потрібно позначити домен або відправника електронної пошти безпечним?</span><span class="sxs-lookup"><span data-stu-id="c72b5-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="c72b5-103">Використання **безпечних списків відправників не рекомендується** , оскільки вона відкриває вашу організацію для спаму, phish і спуфінгу атак.</span><span class="sxs-lookup"><span data-stu-id="c72b5-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="c72b5-104">Однак, якщо є бізнес-вимога, ми **рекомендуємо** використовувати **[правила потоку пошти](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** для цього.</span><span class="sxs-lookup"><span data-stu-id="c72b5-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="c72b5-105">Наші вказівки гарантують автентичність відправника (перевірка домену, який надсилає надсилання, не є підробною).</span><span class="sxs-lookup"><span data-stu-id="c72b5-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="c72b5-106">**Примітка**: не рекомендовано керувати помилковими спрацьовувань за допомогою списків надійних відправників, оскільки винятки з фільтрації спаму можуть відкрити організацію для атак безпеки.</span><span class="sxs-lookup"><span data-stu-id="c72b5-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="c72b5-107">Якщо користувач (и) отримує повідомлення помилково позначено як спам або Небажана пошта, будь ласка, **[повідомляйте про повідомлення та файли до корпорації Майкрософт](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="c72b5-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="c72b5-108">Надійні відправники в Outlook, дозволені список відправників або дозволений список доменів у політиці проти спаму **слід уникати** , оскільки відправники оминають всі спам, пародія і phish Protection та автентифікацію ВІДПРАВНИКА (SPF, DKIM, DKIM).</span><span class="sxs-lookup"><span data-stu-id="c72b5-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="c72b5-109">Цей метод найкраще використовувати тільки для тимчасового тестування.</span><span class="sxs-lookup"><span data-stu-id="c72b5-109">This method is best used for temporary testing only.</span></span>
