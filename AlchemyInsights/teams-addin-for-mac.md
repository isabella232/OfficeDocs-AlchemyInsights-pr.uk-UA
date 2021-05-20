---
title: Teams надбудови для Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582091"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="59a93-102">Teams надбудови для Mac</span><span class="sxs-lookup"><span data-stu-id="59a93-102">Teams add-in for Mac</span></span>

<span data-ttu-id="59a93-103">Щоб усунути відсутніх Teams користувачів операційної системи для Mac, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="59a93-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="59a93-104">**Крок 1.** Якщо використовується гібридне середовище Exchange локальний (2016 CU3 або пізнішої версії), скористайтеся засобом Test-HMA.ps1, щоб переконатися, що гібридну сучасну автентифікацію настроєно правильно.</span><span class="sxs-lookup"><span data-stu-id="59a93-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="59a93-105">Докладні відомості див. в [розділ Перевірка налаштування гібридної сучасної автентифікації Outlook для iOS і Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="59a93-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="59a93-106">**Примітка** Використовуйте формат адреси UPN [(наприклад,](mailto:username@contoso.com)"username@contoso.com"), а не домен\ім'я_користувача.</span><span class="sxs-lookup"><span data-stu-id="59a93-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="59a93-107">Зробіть це навіть для користувачів із Exchange Online поштових скриньок.</span><span class="sxs-lookup"><span data-stu-id="59a93-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="59a93-108">**Крок 2.** Користувач може перейти до меню **Інструменти Облікові**  >  **записи**... у Outlook для Mac, знайдіть і виберіть обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="59a93-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="59a93-109">Переконайтеся, що ім'я користувача зазначено у форматі UPN (наприклад, [username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="59a93-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="59a93-110">**Крок 3.** Переконайтеся, що користувач має ліцензію Microsoft Teams користувача.</span><span class="sxs-lookup"><span data-stu-id="59a93-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="59a93-111">Користувач має використовувати передплату на Office 365 для Mac версії 16.24 або пізнішої.</span><span class="sxs-lookup"><span data-stu-id="59a93-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>