---
title: Команди Microsoft – гостьовий доступ
ms.author: heidip
author: microsoftheidi
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "311"
- "6500001"
ms.openlocfilehash: ee38dcb5f40ea16cea1b84b9b16e86b0f52f2d89
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/13/2020
ms.locfileid: "48452249"
---
# <a name="microsoft-teams---guest-access"></a>Команди Microsoft – гостьовий доступ

Якщо вам потрібна допомога в спілкуванні з користувачами поза межами організації в командах, потрібно вирішити, чи слід використовувати [гостьовий доступ або зовнішній доступ (Федерація)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access), або ви можете використовувати обидва.

Обов'язково ознайомтеся з [відмінностями](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) , щоб дізнатися про функції, доступні для кожного з них.  Наприклад, зовнішній доступ (Федерація) дає змогу для спілкування в 1:1, як-от чат і присутність.  Однак не можна брати участь у роботі робочих груп за допомогою федеративного користувача.  Якщо ви хочете, щоб зовнішній користувач приєднався до участі в групах каналів або надати спільний доступ до файлів, потрібно ввімкнути Гостьове Access.

**Параметр 1: Увімкнення гостьового доступу** У центрі адміністрування команд послідовно виберіть елементи [настройки організаційних параметрів > гостьового](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) доступу та активуйте параметр "Дозволити гостьовий доступ в командах".  Для клієнта з усіма іншими настройками за замовчуванням, це має бути все, що потрібно зробити.  Щоб настроїти конфігурацію гостьового доступу, переконайтеся, що ви виконаєте всі кроки в [контрольному списку гостей Access](https://docs.microsoft.com/microsoftteams/guest-access-checklist). Після того як ви повністю закінчите, потрібно зачекати до [24 годин](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) , щоб параметри набрали сили.

Якщо ви впевнені, що ви виконали всі кроки в контрольному списку, а це було понад 24 години, перейдіть вперед і спробувати [Додати гостя до своєї команди](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop).

Щоб отримати докладні відомості, зокрема про відеоролики, ознайомтеся [з Гостьовим доступом в командах Microsoft](https://docs.microsoft.com/microsoftteams/guest-access).

**Варіант 2: Увімкнення зовнішнього доступу (Федерація)** Якщо ви також хотіли б увімкнути зовнішній доступ (Федерація), у центрі адміністрування груп перейдіть до [параметрів організаційної настройки > зовнішній доступ](https://admin.teams.microsoft.com/company-wide-settings/external-communications) і ввімкніть "користувачі можуть спілкуватися зі службою" Skype для бізнесу "та" для користувачів груп ", а потім виконайте всі кроки, [щоб користувачі групи могли спілкуватися в чаті та спілкуватися з користувачами в іншій організації](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization).
