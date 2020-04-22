---
title: Пенсійні інструменти для Витребування спадщини
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
ms.openlocfilehash: 262cca0feee17d1f929a5a94a4dd6c1ec317f6ec
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/21/2020
ms.locfileid: "43650589"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="a52c6-102">Пенсійні інструменти для Витребування спадщини</span><span class="sxs-lookup"><span data-stu-id="a52c6-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="a52c6-103">У результаті нових і вдосконалених функції Витребування електронної інформації в Microsoft 365 центр відповідності, такі застарілі засоби для Витребування та використання, буде припинено в найближчі місяці:</span><span class="sxs-lookup"><span data-stu-id="a52c6-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="a52c6-104">[Електронне Витребування на місці](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) та його [місце займає](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Центр адміністрування Exchange.</span><span class="sxs-lookup"><span data-stu-id="a52c6-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="a52c6-105">Exchange Online командлети PowerShell, які підтримують на місці, Витребування та на місці, має.</span><span class="sxs-lookup"><span data-stu-id="a52c6-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="a52c6-106">(Ці командлети колективно визначаються як \*-MailboxSearch командлети.) Це включає в себе такі командлети:</span><span class="sxs-lookup"><span data-stu-id="a52c6-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="a52c6-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="a52c6-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="a52c6-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="a52c6-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="a52c6-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="a52c6-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="a52c6-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="a52c6-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="a52c6-111">Командлет [Search-поштової скриньки](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a52c6-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="a52c6-112">Такі операції в API веб-служб Exchange:</span><span class="sxs-lookup"><span data-stu-id="a52c6-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="a52c6-113">Коробки для пошуку по пошті</span><span class="sxs-lookup"><span data-stu-id="a52c6-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="a52c6-114">Поштові скриньки</span><span class="sxs-lookup"><span data-stu-id="a52c6-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="a52c6-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="a52c6-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="a52c6-116">Розширене Витребування електронної інформації v 1.0</span><span class="sxs-lookup"><span data-stu-id="a52c6-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="a52c6-117">**Терміни виходу на пенсію**:</span><span class="sxs-lookup"><span data-stu-id="a52c6-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="a52c6-118">1 квітня 2020: ви не зможете створювати нові пошукові запити та утримані, але ви все одно можете запускати, редагувати та видаляти наявні пошукові запити на власний ризик.</span><span class="sxs-lookup"><span data-stu-id="a52c6-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="a52c6-119">Служба підтримки Microsoft більше не буде підтримувати Витребування на місці, & утримуватиме на рівні.</span><span class="sxs-lookup"><span data-stu-id="a52c6-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="a52c6-120">1 липня 2020: на місці Витребування електронної & тримає функціональність в EАС буде поміщений в режимі лише для читання.</span><span class="sxs-lookup"><span data-stu-id="a52c6-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="a52c6-121">Це означає, що ви зможете лише видалити наявні пошукові запити та утримань.</span><span class="sxs-lookup"><span data-stu-id="a52c6-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="a52c6-122">**Для отримання додаткових відомостей див**.:</span><span class="sxs-lookup"><span data-stu-id="a52c6-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="a52c6-123">Міграція застарілих пошук Витребування та утримань до Microsoft 365 центр відповідності</span><span class="sxs-lookup"><span data-stu-id="a52c6-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="a52c6-124">Пенсійні інструменти для Витребування спадщини</span><span class="sxs-lookup"><span data-stu-id="a52c6-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="a52c6-125">Запитання й відповіді про місце Витребування на місці та утримань на місці</span><span class="sxs-lookup"><span data-stu-id="a52c6-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



