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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Пенсійні інструменти для Витребування спадщини

У результаті нових і вдосконалених функції Витребування електронної інформації в Microsoft 365 центр відповідності, такі застарілі засоби для Витребування та використання, буде припинено в найближчі місяці:

- [Електронне Витребування на місці](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) та його [місце займає](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Центр адміністрування Exchange.

- Exchange Online командлети PowerShell, які підтримують на місці, Витребування та на місці, має. (Ці командлети колективно визначаються як *-MailboxSearch командлети.) Це включає в себе такі командлети:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Командлет [Search-поштової скриньки](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) в Exchange Online PowerShell.
- Такі операції в API веб-служб Exchange:
    - [Коробки для пошуку по пошті](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Поштові скриньки](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Розширене Витребування електронної інформації v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Терміни виходу на пенсію**:
- 1 квітня 2020: ви не зможете створювати нові пошукові запити та утримані, але ви все одно можете запускати, редагувати та видаляти наявні пошукові запити на власний ризик. Служба підтримки Microsoft більше не буде підтримувати Витребування на місці, & утримуватиме на рівні.

- 1 липня 2020: на місці Витребування електронної & тримає функціональність в EАС буде поміщений в режимі лише для читання. Це означає, що ви зможете лише видалити наявні пошукові запити та утримань.

**Для отримання додаткових відомостей див**.:

 - [Міграція застарілих пошук Витребування та утримань до Microsoft 365 центр відповідності](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Пенсійні інструменти для Витребування спадщини](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Запитання й відповіді про місце Витребування на місці та утримань на місці](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



