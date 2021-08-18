---
title: Використання Giphys у Teams розмовах
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 296c2f80d35f1c93ab3c60e0be65fd96c953ca81
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323541"
---
# <a name="using-giphys-in-teams-conversations"></a>Використання Giphys у Teams розмовах

Доступ до Giphys Teams чаті ввімкнуто за замовчуванням. Як адміністратор ви можете керувати доступністю Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) користувачам, установивши політику обміну повідомленнями та перевіривши, чи ввімкнуто параметр Використовувати **Giphys у** **розмовах.**

Якщо під час розмов Teams не працюють гіфунично-об'Teams, перевірте:

Політика [обміну повідомленнями повинна](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) дозволити Giphys. Перевірка за допомогою командлетів PowerShell

- Переконайтеся, що ви [можете керувати Teams за допомогою PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Виконайте команду PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) і переконайтеся, що **для параметра AllowGiphy** установлено **значення TRUE.**
- Якщо **для параметра AllowGiphy** установлено **значення FALSE**, виконайте таку команду PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Щоб надати доступ до](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) URL-адреси Giphy, потрібно ввімкнути підключені можливості.

**Примітка.** Якщо для вашого клієнта настроєно кілька політик обміну повідомленнями Teams, можна визначити ідентичність політики, призначеної відповідному користувачу за допомогою команди PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Виберіть TeamsMessagingPolicy.
