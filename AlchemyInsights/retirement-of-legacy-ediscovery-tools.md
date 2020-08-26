---
title: Вихід із програми «застарілі засоби пошуку»
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902641"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="3481e-102">Вихід із програми «застарілі засоби пошуку»</span><span class="sxs-lookup"><span data-stu-id="3481e-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="3481e-103">У результаті нової та покращеної функції eDiscovery в центрі відповідності Microsoft 365 наведені нижче застарілі Знаряддя для виявлення та командлетів будуть списані в наступні місяці:</span><span class="sxs-lookup"><span data-stu-id="3481e-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="3481e-104">На місці Витребування [електронної](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) інформації та [на місці тримає](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центрі адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="3481e-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="3481e-105">Командлети Exchange Online, які підтримують підтримку на місці та на місці.</span><span class="sxs-lookup"><span data-stu-id="3481e-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="3481e-106">(Ці командлети в сукупності визначаються як командлети \*-MailboxSearch). Це включає такі командлети:</span><span class="sxs-lookup"><span data-stu-id="3481e-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="3481e-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3481e-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="3481e-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3481e-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="3481e-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3481e-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="3481e-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="3481e-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="3481e-111">Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) у службі Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3481e-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="3481e-112">Нижче наведено дії, описані в API веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="3481e-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="3481e-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="3481e-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="3481e-114">Поштові скриньки SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="3481e-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="3481e-115">Поштові скриньки getholdon</span><span class="sxs-lookup"><span data-stu-id="3481e-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="3481e-116">Розширені можливості eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="3481e-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="3481e-117">**Часова шкала для виходу на пенсію**:</span><span class="sxs-lookup"><span data-stu-id="3481e-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="3481e-118">**1 липня 2020 р** . Ви більше не можете створювати нові пошукові запити та виконувати, але ви можете запускати, редагувати та видаляти поточні пошуки на власний ризик.</span><span class="sxs-lookup"><span data-stu-id="3481e-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="3481e-119">Служба підтримки корпорації Майкрософт більше не підтримує функцію "Діскавері" на місці, & проводить в "eDiscovery".</span><span class="sxs-lookup"><span data-stu-id="3481e-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="3481e-120">**1 жовтня 2020 р** . Функція eDiscovery & містить функції, які можна буде розташувати в режимі лише для читання, щоб ви могли видалити лише доступні пошукові запити та утримання.</span><span class="sxs-lookup"><span data-stu-id="3481e-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="3481e-121">**Докладні відомості наведено в статті**:</span><span class="sxs-lookup"><span data-stu-id="3481e-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="3481e-122">Перенесення попередніх результатів пошуку в службі виявлення та утримання в центрі відповідності Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="3481e-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="3481e-123">Вихід із програми «застарілі засоби пошуку»</span><span class="sxs-lookup"><span data-stu-id="3481e-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="3481e-124">Запитання й відповіді про неавтоматичний пошук і проведення на місці</span><span class="sxs-lookup"><span data-stu-id="3481e-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



