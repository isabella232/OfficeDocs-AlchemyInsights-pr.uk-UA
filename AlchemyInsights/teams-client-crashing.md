---
title: Клієнт Teams аварійно завершує роботу?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354074"
---
# <a name="teams-client-crashing"></a>Клієнт Teams аварійно завершує роботу?

Якщо клієнт Teams аварійно завершує роботу, виконайте наведені нижче дії.

- Якщо ви використовуєте класичну версію програми Teams, [переконайтеся, що її повністю оновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Переконайтеся, що всі [URL-адреси Microsoft 365 і діапазони адрес](https://docs.microsoft.com/microsoftteams/connectivity-issues) доступні.

- Увійдіть у систему з обліковим записом адміністратора клієнта та перевірте [приладну дошку справності](https://docs.microsoft.com/office365/enterprise/view-service-health) , щоб перевірити, чи існує відсутність перебої або погіршення служби.

- Видаліть і переінсталюйте програму teams (посилання)
    - Перейдіть до%Appded%\mice\systems\ папки на комп'ютері та видалити всі файли в цьому каталозі.
    - [Скачайте і встановіть додаток teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), і, якщо можливо, встановіть teams як адміністратор (клацніть правою кнопкою миші інсталятор команд і виберіть "Запуск від як адміністратор", якщо доступно).

Якщо ваш клієнт команди все ще збій, ви можете відтворити проблему? Якщо так:

1. Використовуйте засіб записування дій, щоб захопити ваші дії.
    - Закрийте всі непотрібні або конфіденційні програми.
    - Запустіть засіб записування дій і відтворити проблему, під час входу з відповідного облікового запису користувача.
    - [Зберіть команди журналів, які захоплюють записані відтворення зв кроки](https://docs.microsoft.com/microsoftteams/log-files). **Зверніть увагу**: переконайтеся, що ви захоплення входу адресу впливу користувача.
    - Збір дампа і/або несправність інформації відро (Windows). Запустіть Windows PowerShell на комп'ютері, де відбувається збій і виконайте такі команди:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Прикріпіть файл до справи підтримки.
