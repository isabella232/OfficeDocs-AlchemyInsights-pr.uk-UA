---
title: Microsoft Teams- Гостьовий доступ
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
ms.openlocfilehash: 2c78fec14d43c5cbf6aebbc889d606eb2f6c4c64af85997f523d06872c911a0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012329"
---
# <a name="microsoft-teams---guest-access"></a>Microsoft Teams- Гостьовий доступ

Якщо вам потрібна допомога з спілкуванням із користувачами за межами організації в Teams, вам потрібно вирішити, чи використовувати гостьовий доступ, зовнішній доступ [(федерація)](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access)або обидва варіанти.

Обов'язково [перегляньте відмінності, щоб](https://docs.microsoft.com/microsoftteams/manage-external-access#external-access-vs-guest-access) зрозуміти функції, доступні для кожного з них.  Наприклад, зовнішній доступ (федерація) дає змогу спілкуватися без підключення до мережі "Один-до-одного", наприклад "Чат" і "Присутність".  Проте федеративні користувачі не можуть Teams співпрацювати.  Якщо потрібно, щоб зовнішній користувач приєднався до розмов у каналі Teams або надав спільний доступ до файлів, увімкніть гостьовий доступ.

**Варіант 1. Увімкнення гостьового доступу** У Центрі Teams адміністрування перейдіть до [](https://admin.teams.microsoft.com/company-wide-settings/guest-configuration) групи Настройки > Гостьовий доступ і ввімкніть параметр "Дозволити гостьовий доступ у Teams".  Це потрібно зробити лише для клієнта з іншими стандартними параметрами.  Щоб налаштувати конфігурацію гостьового доступу, обов'язково виконайте всі дії, описані в [контрольного списку Гостьовий доступ.](https://docs.microsoft.com/microsoftteams/guest-access-checklist) Коли все буде готово, зачекайте [24](https://docs.microsoft.com/microsoftteams/manage-guests#guest-access-latencies) години, щоб настройки набрали сили.

Якщо ви впевнені, що ви виконили всі кроки в контрольний список і вже понад 24 години, спробуйте додати гостя до робочої [групи.](https://support.office.com/article/add-guests-to-a-team-in-teams-fccb4fa6-f864-4508-bdde-256e7384a14f#ID0EAABAAA=Desktop)

Докладні відомості, зокрема відео інструкції, див. в статті [Гостьовий доступ Microsoft Teams](https://docs.microsoft.com/microsoftteams/guest-access).

**Варіант 2. Увімкнення зовнішнього доступу (федерації)** Якщо потрібно ввімкнути зовнішній доступ (федерацію), у Центрі адміністрування Teams перейдіть на сторінку Зовнішній доступ Настройки > для всієї організації [та](https://admin.teams.microsoft.com/company-wide-settings/external-communications) ввімкніть параметр "Користувачі можуть спілкуватися з користувачами Skype для бізнесу і Teams", а потім виконайте всі дії, описані в статті Надання користувачам доступу до [служби Teams](https://docs.microsoft.com/microsoftteams/manage-external-access#let-your-teams-users-chat-and-communicate-with-users-in-another-organization)і спілкування з користувачами в іншій організації.
