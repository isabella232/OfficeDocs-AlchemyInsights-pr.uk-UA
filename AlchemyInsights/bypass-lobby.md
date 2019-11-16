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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768461"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Контроль параметрів лобі та рівень участі

Якщо ви хочете дозволити всім, зокрема, комутованих, зовнішніх і анонімних користувачів, щоб обійти фойє у Microsoft teams, ви можете використовувати PowerShell, щоб зробити це. Нижче наведено приклад змінення політики глобального наради для вашої організації.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Цю команду в даний час вимагає використання Skype для бізнесу PowerShell модуль. Щоб отримати параметри для використання цього командлета, перевірте [керування політиками за допомогою PowerShell](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Ви можете створити нову політику, яку потрібно буде застосувати до користувачів. Якщо ви змінюєте глобальну політику, вона автоматично застосовуватиметься до користувачів. Для будь-яких змін в політиці необхідно почекати принаймні 4 години і до 24 годин, щоб політика набрали сили.

Обов'язково перегляньте документацію нижче, перш ніж вносити ці зміни, щоб точно зрозуміти, що це дозволяє.

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Знайомство з командами переговорних елементів керування політикою

- [Автоматично визнати](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , що люди в політиці для Організатора, що контролює, чи є люди приєднатися до наради безпосередньо або чекати у фойє, поки вони не будуть допущені автентифікованим користувачем.

- [Дозволити анонімним людям розпочати нараду](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) – це політика Організатора, яка керує тим, чи можуть користувачі анонімних користувачів, ВКЛЮЧНО з B2B та федеративними користувачами, приєднатися до наради користувача без автентифікованого користувача з організації.

- [Дозволити комутованого користувачів, щоб обійти фойє](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) є для Організатора політики, яка контролює, чи люди, які підключаються по телефону приєднатися до наради безпосередньо або чекати в холі, незалежно від того, **автоматично визнати, люди** налаштування.

- [Дозволити організаторам змінювати параметри фойє](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**скоро**)-це політика Організатора, яка керує тим, чи може Організатор наради перевизначити параметри фойє, які встановлюються адміністратором у **автоматичному режимі, допускають** користувачів і **дозволяють користувачам телефонувати до фойє** під час планування нової наради.

**Примітка:** Для повного огляду політики зборів Microsoft teams прочитайте [команди керування політикою нарад](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) .
