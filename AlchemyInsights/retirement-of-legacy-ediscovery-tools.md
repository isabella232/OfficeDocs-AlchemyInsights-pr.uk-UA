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
# <a name="retirement-of-legacy-ediscovery-tools"></a>Вихід із програми «застарілі засоби пошуку»

У результаті нової та покращеної функції eDiscovery в центрі відповідності Microsoft 365 наведені нижче застарілі Знаряддя для виявлення та командлетів будуть списані в наступні місяці:

- На місці Витребування [електронної](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) інформації та [на місці тримає](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) в центрі адміністрування Exchange.

- Командлети Exchange Online, які підтримують підтримку на місці та на місці. (Ці командлети в сукупності визначаються як командлети *-MailboxSearch). Це включає такі командлети:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Командлет [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) у службі Exchange Online PowerShell.
- Нижче наведено дії, описані в API веб-служб Exchange:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Поштові скриньки SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Поштові скриньки getholdon](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Розширені можливості eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Часова шкала для виходу на пенсію**:
- **1 липня 2020 р** . Ви більше не можете створювати нові пошукові запити та виконувати, але ви можете запускати, редагувати та видаляти поточні пошуки на власний ризик. Служба підтримки корпорації Майкрософт більше не підтримує функцію "Діскавері" на місці, & проводить в "eDiscovery".
    
- **1 жовтня 2020 р** . Функція eDiscovery & містить функції, які можна буде розташувати в режимі лише для читання, щоб ви могли видалити лише доступні пошукові запити та утримання.

**Докладні відомості наведено в статті**:

 - [Перенесення попередніх результатів пошуку в службі виявлення та утримання в центрі відповідності Microsoft 365](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Вихід із програми «застарілі засоби пошуку»](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Запитання й відповіді про неавтоматичний пошук і проведення на місці](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



