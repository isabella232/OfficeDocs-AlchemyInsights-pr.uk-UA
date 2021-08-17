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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104329"
---
# <a name="using-giphys-in-teams-conversations"></a>Використання Giphys у Teams розмовах

Доступ до Giphys Teams чаті ввімкнуто за замовчуванням. Як адміністратор ви можете керувати доступністю Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) користувачам, установивши політику обміну повідомленнями та перевіривши, чи ввімкнуто параметр Використовувати **Giphys у** **розмовах.**

Якщо під час розмов Teams не працюють гіфами, перевірте:

Політика [обміну повідомленнями повинна](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) дозволити Giphys. Перевірка за допомогою командлетів PowerShell

- Переконайтеся, що ви [можете керувати Teams за допомогою PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Виконайте команду PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) і переконайтеся, що **для параметра AllowGiphy** установлено значення **TRUE.**
- Якщо **для параметра AllowGiphy** установлено **значення FALSE**, виконайте таку команду PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Щоб надати доступ до](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) URL-адреси Giphy, потрібно ввімкнути підключені можливості.

> [!NOTE]
> Якщо для вашого клієнта настроєно кілька політик обміну повідомленнями Teams, можна визначити ідентичність політики, призначеної відповідному користувачу за допомогою команди PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Виберіть TeamsMessagingPolicy.
