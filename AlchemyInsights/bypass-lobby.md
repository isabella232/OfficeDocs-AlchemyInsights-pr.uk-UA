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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376897"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>Контроль параметрів лобі та рівень участі

Ці настройки керують тим, що учасники зустрічі чекають у вестибюлі, перш ніж вони будуть допущені до зустрічі і рівень участі, який вони можуть отримати на нараді. PowerShell можна використовувати для оновлення зустрічі параметри політики, які ще не реалізовано (з написом "скоро") у команди центру адміністрування.  Нижче наведено приклад командлета PowerShell, який дозволяє всім користувачам обходити фойє.  

- [Автоматично визнати](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) , що люди в політиці для Організатора, що контролює, чи є люди приєднатися до наради безпосередньо або чекати у фойє, поки вони не будуть допущені автентифікованим користувачем.

- [Дозволити анонімним людям розпочати нараду](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) – це політика Організатора, яка керує тим, чи можуть користувачі анонімних користувачів, ВКЛЮЧНО з B2B та федеративними користувачами, приєднатися до наради користувача без автентифікованого користувача з організації.

- [Дозволити комутованого користувачів, щоб обійти фойє](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**скоро**) є для Організатора політики, яка контролює, чи люди, які підключаються по телефону приєднатися до наради безпосередньо або чекати в холі, незалежно від того, **автоматично визнати, люди** налаштування.

- [Дозволити організаторам змінювати параметри фойє](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**скоро**)-це політика Організатора, яка керує тим, чи може Організатор наради перевизначити настройки фойє, які встановлюються адміністратором у **автоматичному режимі** ** користувачі, щоб обійти фойє** під час планування нової наради.

**Примітка:** Для повного огляду політики зборів Microsoft teams прочитайте [команди керування політикою нарад](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) . 


**Приклад PowerShell**

Якщо ви хочете дозволити всім, включаючи зовнішніх або анонімних користувачів, обійти фойє, ви також можете використовувати PowerShell для виконання цього завдання.  Нижче наведено приклад змінення політики глобального наради для вашої організації.   

(Обов'язково перегляньте документацію вище, перш ніж вносити ці зміни, щоб точно зрозуміти, що це дозволяє.)

Набір-Cпароплавполітика-ідентичність Global-AutoAdmittedUsers "все"-Дозволяєредагувати $True

Щоб отримати додаткові відомості, [див.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)
