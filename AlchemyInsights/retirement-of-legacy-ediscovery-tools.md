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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Відновлення застарілих засобів витребування електронної даних

У результаті нових і вдосконалених функцій витребування електронної даних у Центрі відповідності Microsoft 365 ми закриємо такі застарілі засоби й командлети для витребування електронної пошти в найближчі місяці:

- [Витребування електронної](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) пошти на місці та утримання на місці [в](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Центрі адміністрування Exchange.

- Командлети Exchange Online PowerShell, які підтримують In-Place витребування In-Place витребування електронної In-Place даних. (Ці командлети спільно визначено як командлети *-MailboxSearch). До них відносяться такі командлети:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) (Поштова скринька пошуку) в Exchange Online PowerShell.
- У API веб-служб Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Часової шкали для виводу з обіду:**
- **1 липня 2020 р.** Більше не можна створювати нові пошукові запити й утримувати їх, але ви можете запускати, редагувати й видаляти наявні пошукові запити на власний ризик. Служба підтримки Microsoft більше не підтримує In-Place витребування & в EAC.
    
- 1 жовтня **2020** In-Place року функції витребування & утримання для витребування електронної інформації в EAC будуть розміщуватись у режимі лише для читання, тому наявні пошукові запити й утримання можна видалити лише.

**Докладні відомості див. в такому:**

 - [Перенесення застарілих пошукових запитів витребування електронної даних у Центрі відповідності Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Відновлення застарілих засобів витребування електронної даних](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Запитання й відповіді про утримання In-Place витребування In-Place електронної інформації](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



