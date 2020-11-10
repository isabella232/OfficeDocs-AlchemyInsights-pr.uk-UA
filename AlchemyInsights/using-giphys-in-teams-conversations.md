---
title: Використання Гіфіз в розмовах команд
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982573"
---
# <a name="using-giphys-in-teams-conversations"></a>Використання Гіфіз в розмовах команд

Підтримка giphys у чаті команд активовано за замовчуванням. Адміністратор може визначати, чи доступні для користувачів Giphys, [настроївши політику обміну повідомленнями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) та **гарантуючи, що** в них **використовується функція giphys** .

Якщо GIF-файли не працюють належним чином в розмовах зі командами, перевірте:

[Політика обміну повідомленнями](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) має дозволити giphys. Щоб перевірити за допомогою командлетів PowerShell, виконайте наведені нижче дії.

- Переконайтеся, що ви можете [керувати командами за допомогою PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Запустіть команду "Завантажити", щоб [отримати доступ](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) до цієї програми, щоб визначити, що **AllowGiphy** має значення **True**.
- Якщо **AllowGiphy** має значення **false** , виконайте наведені нижче набір команд PowerShell [– значення політики глобального – AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

Щоб дозволити доступ до URL-адреси Giphy, потрібно ввімкнути [додатковий підключений досвід](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) .

> [!NOTE]
> Якщо у вас є кілька політик обміну повідомленнями групи, настроєні для вашого клієнта, можна визначити ідентичність політики, призначеної для певного користувача за допомогою команди PowerShell [Get-CsOnlineUser-Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Виберіть команду TeamsMessagingPolicy.
