---
title: Надбудова "команди" для Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630023"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="f50a4-102">Надбудова "команди" для Mac</span><span class="sxs-lookup"><span data-stu-id="f50a4-102">Teams add-in for Mac</span></span>

<span data-ttu-id="f50a4-103">Щоб виправити неполадки в надбудові відсутніх груп для користувачів операційної системи Mac, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="f50a4-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="f50a4-104">**Крок 1:** Якщо у вас є гібридний локальний Exchange (2016 CU3 або пізніша версія), скористайтеся засобом Test-HMA.ps1, щоб підтвердити, що ця гібридна сучасна автентифікація правильно настроєно.</span><span class="sxs-lookup"><span data-stu-id="f50a4-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="f50a4-105">Докладні відомості наведено в статті [перевірка гібридної версії сучасної автентифікації для програми Outlook для IOS і Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="f50a4-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="f50a4-106">**Примітка** . Використовуйте формат адреси для UPN (наприклад, [username@contoso.com](mailto:username@contoso.com)), а не домен \ ім'я _ користувача.</span><span class="sxs-lookup"><span data-stu-id="f50a4-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="f50a4-107">Зробіть це навіть для користувачів із поштовими скриньками Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="f50a4-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="f50a4-108">**Крок 2:** Маєте користувача перейти до **Tools**  >  **облікових записів**Tools... у програмі Outlook для Mac і знайдіть і виберіть обліковий запис.</span><span class="sxs-lookup"><span data-stu-id="f50a4-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="f50a4-109">Переконайтеся, що ім'я користувача вказано в форматі UPN (наприклад, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="f50a4-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="f50a4-110">**Крок 3:** Підтвердьте, що користувач – це ліцензований користувач групи Microsoft.</span><span class="sxs-lookup"><span data-stu-id="f50a4-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="f50a4-111">Користувач має використовувати передплатою Office 365 для Mac, версію продукту 16,24 або пізнішу.</span><span class="sxs-lookup"><span data-stu-id="f50a4-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>