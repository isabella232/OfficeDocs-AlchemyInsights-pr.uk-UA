---
title: Обійти фойє
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820055"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Керування параметрами фойє та рівнем участі в Teams

Щоб обійти фойє, скористайтеся PowerShell, щоб виконати це завдання, якщо потрібно дозволити всім, зокрема вхідні, зовнішні та анонімні користувачі.  Ось приклад змінення глобальної політики наради для організації.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Цей командлет наразі потребує використання модуля PowerShell служби "Skype для бізнесу". Щоб налаштувати використання цього командлета, ознайомтесь із цією цією командлетом, щоб дізнатися про керування [політиками за допомогою PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Після налаштування політики її потрібно застосувати до користувачів. або, якщо ви змінили політику Global, вона автоматично застосовуватиме до користувачів. Щоб політики набрали сили, зачекайте принаймні 4 години до **24** годин. 

Обов'язково перегляньте наведену нижче документацію, перш ніж вносити ці зміни, щоб зрозуміти, що це дозволяє.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Докладні відомості про елементи керування політикою "фойє" наради Teams

Ці параметри керують тим, які учасники наради чекають у фойє, перш ніж їх буде прийнято на нараду, і рівень участі, які вони можуть брати на нараду. За допомогою PowerShell можна оновити параметри політики нарад, які ще не впроваджено (з позначкою "незабаром") у Центрі адміністрування Teams. Нижче наведено приклад командлета PowerShell, який дає змогу всім користувачам обійти фойє.

- [Автоматично допускати](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) користувачів – це політика кожного організатора, яка визначає, чи користувачі можуть безпосередньо приєднуватися до наради, або чекати у "фойє", доки автентифікований користувач не приєднається до наради.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Дозволити анонімним користувачам розпочинати нараду – це політика кожного організатора, яка визначає, чи можуть анонімні користувачі, зокрема B2B та федеративні користувачі, приєднатися до наради користувача без автентифікованого користувача з організації під час відвідування.

- Дозволити [користувачам-організаторам](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) обходити фойє **(очікується** незабаром) – це політика від кожного організатора, яка визначає, чи користувачі, які приєднаються  по телефону, можуть безпосередньо приєднатися до наради або чекати у фойє незалежно від параметра Автоматично допускати користувачів.

- Дозволити організаторам перевизначати настройки фойє (незабаром) – це політика кожного організатора, яка визначає, чи може  організатор наради  перевизначати параметри фойє, установлені адміністратором у розділі Автоматичне допускання користувачів і Надання користувачам дозволу оминати фойє під час планування нової наради. [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) 

**Примітка.** Повний [огляд політик нарад Microsoft Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) див. в статті Керування політиками нарад у Teams.
