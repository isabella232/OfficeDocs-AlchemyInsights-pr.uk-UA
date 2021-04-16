---
title: Відновлення застарілих засобів витребування електронної даних
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798570"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="d3f35-102">Відновлення застарілих засобів витребування електронної даних</span><span class="sxs-lookup"><span data-stu-id="d3f35-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="d3f35-103">У результаті нових і вдосконалених функцій витребування електронної даних у Центрі відповідності Microsoft 365 ми закриємо такі застарілі засоби й командлети для витребування електронної пошти в найближчі місяці:</span><span class="sxs-lookup"><span data-stu-id="d3f35-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="d3f35-104">[Витребування електронної](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) пошти на місці та утримання на місці [в](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Центрі адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="d3f35-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="d3f35-105">Командлети Exchange Online PowerShell, які підтримують In-Place витребування In-Place витребування електронної In-Place даних.</span><span class="sxs-lookup"><span data-stu-id="d3f35-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="d3f35-106">(Ці командлети спільно визначено як командлети \*-MailboxSearch). До них відносяться такі командлети:</span><span class="sxs-lookup"><span data-stu-id="d3f35-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="d3f35-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d3f35-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="d3f35-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d3f35-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="d3f35-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d3f35-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="d3f35-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d3f35-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="d3f35-111">Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) (Поштова скринька пошуку) в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d3f35-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="d3f35-112">У API веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="d3f35-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="d3f35-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d3f35-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="d3f35-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d3f35-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="d3f35-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d3f35-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="d3f35-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="d3f35-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="d3f35-117">**Часової шкали для виводу з обіду:**</span><span class="sxs-lookup"><span data-stu-id="d3f35-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="d3f35-118">**1 липня 2020 р.** Більше не можна створювати нові пошукові запити й утримувати їх, але ви можете запускати, редагувати й видаляти наявні пошукові запити на власний ризик.</span><span class="sxs-lookup"><span data-stu-id="d3f35-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="d3f35-119">Служба підтримки Microsoft більше не підтримує In-Place витребування & в EAC.</span><span class="sxs-lookup"><span data-stu-id="d3f35-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="d3f35-120">1 жовтня **2020** In-Place року функції витребування & утримання для витребування електронної інформації в EAC будуть розміщуватись у режимі лише для читання, тому наявні пошукові запити й утримання можна видалити лише.</span><span class="sxs-lookup"><span data-stu-id="d3f35-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="d3f35-121">**Докладні відомості див. в такому:**</span><span class="sxs-lookup"><span data-stu-id="d3f35-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="d3f35-122">Перенесення застарілих пошукових запитів витребування електронної даних у Центрі відповідності Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="d3f35-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="d3f35-123">Відновлення застарілих засобів витребування електронної даних</span><span class="sxs-lookup"><span data-stu-id="d3f35-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="d3f35-124">Запитання й відповіді про утримання In-Place витребування In-Place електронної інформації</span><span class="sxs-lookup"><span data-stu-id="d3f35-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



