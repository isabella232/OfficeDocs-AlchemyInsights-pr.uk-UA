---
title: Обійти лобі
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889103"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Контроль параметрів лобі та рівень участі в teams

Якщо ви хочете дозволити всім, включаючи комутованих, зовнішніх і анонімних користувачів, щоб **обійти фойє**, використовуйте PowerShell для виконання цього завдання. Нижче наведено приклад змінення політики глобального наради для вашої організації.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Цю команду в даний час вимагає використання Skype для бізнесу PowerShell модуль. Щоб отримати налаштування для використання цього командлета, перегляньте [керування політиками за допомогою PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Після настроювання політики потрібно застосувати його до користувачів; або, якщо ви змінили глобальну політику, вона буде автоматично застосовуватися до користувачів. Для будь-яких змін у політиці потрібно зачекати принаймні **4 години до 24 годин** , щоб правила набрали сили. 

Обов'язково перегляньте документацію нижче, перш ніж вносити ці зміни, щоб точно зрозуміти, що це дозволяє.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Знайомство з командами переговорних елементів керування політикою

Ці настройки керують тим, що учасники зустрічі чекають у вестибюлі, перш ніж вони будуть допущені до зустрічі і рівень участі, який вони можуть отримати на нараді. PowerShell можна використовувати для оновлення зустрічі параметри політики, які ще не реалізовано (з написом "скоро") у команди центру адміністрування. Нижче наведено приклад командлета PowerShell, який дозволяє всім користувачам обходити фойє.

- [Автоматично визнати](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , що люди в політиці для Організатора, що контролює, чи є люди приєднатися до наради безпосередньо або чекати у фойє, поки вони не будуть допущені автентифікованим користувачем.

- [Дозволити анонімним людям розпочати нараду](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) – це політика Організатора, яка керує тим, чи можуть користувачі анонімних користувачів, ВКЛЮЧНО з B2B та федеративними користувачами, приєднатися до наради користувача без автентифікованого користувача з організації.

- [Дозволити комутованого користувачів, щоб обійти фойє](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) є для Організатора політики, яка контролює, чи люди, які підключаються по телефону приєднатися до наради безпосередньо або чекати в холі, незалежно від того, **автоматично визнати, люди** налаштування.

- [Дозволити організаторам змінювати параметри фойє](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**скоро**)-це політика Організатора, яка керує тим, чи може Організатор наради перевизначити параметри фойє, які встановлюються адміністратором у **автоматичному режимі, допускають** користувачів і **дозволяють користувачам телефонувати до фойє** під час планування нової наради.

**Примітка:** Для повного огляду політики зборів Microsoft teams прочитайте [команди керування політикою нарад](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) .
