---
title: Обхід лобі
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684971"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Керування параметрами лобі та рівнем участі в командах

Щоб дозволити всім, зокрема використовувати комутоване, зовнішні та анонімні користувачі, щоб **обійти фойє**, використовуйте PowerShell, щоб виконати це завдання. Нижче наведено приклад змінення політики глобального наради для вашої організації.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Цей командлет зараз вимагає використання модуля "Skype для бізнесу PowerShell". Щоб налаштувати використання цього командлета, перегляньте [керування політиками за допомогою PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Коли ви настроїли політику, потрібно використати її для користувачів; або, якщо ви змінили глобальну політику, вона автоматично застосуться до користувачів. Для будь-якої зміни політики потрібно зачекати щонайменше **4 години до 24 годин** , щоб політики набрали сили. 

Обов'язково ознайомтеся з документацією нижче, перш ніж вносити ці зміни, щоб точно розуміти, що це дозволяє.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Загальні відомості про елементи керування "лобіювання політики" в командах нарад

Ці параметри керують тим, що Учасники наради очікують у фойє, перш ніж вони будуть допущені до наради, а рівень участі, яке їм дозволено під час наради. За допомогою PowerShell можна оновити настройки політики наради, які ще не реалізовано (з позначкою "Coming Soon") у центрі адміністрування команд. Нижче наведено приклад командлет PowerShell, який дає змогу всім користувачам обходити вестибюль.

- [Автоматично визнавати людей](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) – це політика для Організатора, яка керує тим, що користувачі можуть приєднатися до наради безпосередньо або чекати в холі, доки вони не будуть допущені автентифікованим користувачем.

- [Дозволити анонімним користувачам почати нараду](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) – це політика для Організатора, яка керує тим, що користувачі, зокрема B2B та федеративного користувачів, можуть приєднатися до наради користувача без автентифікованого користувача в організації.

- [Дозволити користувачам](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) , які не мають права на вхід у вестибюлі (**незабаром**) – це політика для Організатора, яка керує тим, що користувачі, які телефонають за допомогою телефону, можуть приєднатися до наради безпосередньо або чекати в холі, незалежно від того, чи **автоматично визнають користувачів** настройку.

- [Дозволити організаторам змінювати настройки лобі](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**незабаром**) – це політика для Організатора, яка керує тим, що Організатор наради може змінити настройки лобі, які настроєно адміністратором, щоб **автоматично визнавати** **користувачів і дозволити користувачам комутованого з них обходити вестибюль** під час планування нової наради.

**Примітка.** Прочитайте [керування політиками нарад в командах](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) для повного огляду політик нарад Microsoft.
