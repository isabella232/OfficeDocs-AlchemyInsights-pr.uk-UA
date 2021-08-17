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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074701"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Відновлення застарілих засобів витребування електронної даних

У результаті нових і вдосконалених функцій витребування електронної даних у Центрі відповідності Microsoft 365, у найближчі місяці буде вилучено такі застарілі засоби й командлети для витребування електронної пошти:

- [Утримання на](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) місці витребування електронної Exchange на місці. [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- Командлети Exchange Online PowerShell, які підтримують In-Place витребування In-Place витребування електронної In-Place даних. (Ці командлети спільно визначено як командлети *-MailboxSearch). До них відносяться такі командлети:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) (Поштова скринька пошуку Exchange Online PowerShell).
- У наведених нижче операціях у Exchange API веб-служб:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Часової шкали для виводу з обіду:**
- **1 липня 2020 р.** Більше не можна створювати нові пошукові запити й утримувати їх, але ви можете запускати, редагувати й видаляти наявні пошукові запити на власний ризик. Служба підтримки Microsoft більше не підтримує In-Place витребування & в EAC.
    
- 1 жовтня **2020** In-Place року функції витребування & утримання для витребування електронної інформації в EAC будуть розміщуватись у режимі лише для читання, тому наявні пошукові запити й утримання можна видалити лише.

**Докладні відомості див. в такому:**

 - [Перенесення застарілих пошукових запитів витребування електронної Центр відповідності Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Відновлення застарілих засобів витребування електронної даних](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Запитання й відповіді про утримання In-Place витребування In-Place електронної інформації](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



