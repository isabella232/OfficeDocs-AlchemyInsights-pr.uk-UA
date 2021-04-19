---
title: Клієнт Teams аварійно завершує роботу?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826292"
---
# <a name="teams-client-crashing"></a>Клієнт Teams аварійно завершує роботу?

Якщо клієнт Teams аварійно завершує роботу, виконайте наведені нижче дії.

- Якщо ви використовуєте класичну версію програми Teams, [переконайтеся, що її повністю оновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Переконайтеся, що всі URL-адреси та діапазони адрес [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) доступні.

- Увійдіть під обліковим записом адміністратора клієнта та перевірте приладну дошку справності служби, щоб переконатися, що немає перебоїв або погіршення якості служби. [](https://docs.microsoft.com/office365/enterprise/view-service-health)

- Видалення та повторна установка програми Teams (посилання)
    - Перейдіть до папки %appdata%\Microsoft\teams\ на комп'ютері та видаліть усі файли з цього каталогу.
    - [Завантажте](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)та інсталюйте Програму Teams і, якщо це можливо, інсталюйте Teams як адміністратор (клацніть правою кнопкою миші інсталятор Teams і виберіть "Запустити із правами адміністратора", якщо вона доступна).

Чи можна відтворити проблему, якщо клієнт Teams аварійно завершує роботу? Якщо так:

1. Щоб записати кроки, скористайтеся записуванням дій.
    - Закрийте всі непотрібні або конфіденційні програми.
    - Запустіть записувач кроків і відтворіть цю проблему під час входу за допомогою відповідного облікового запису користувача.
    - [Зберіть журнали команд, у яких записано кроки повторного відтворення.](https://docs.microsoft.com/microsoftteams/log-files) **Примітка.** Обов'язково запишіть адресу для входу потрібного користувача.
    - Зберіть дамп і/або відомості про блоки помилок (Windows). Запустіть Windows PowerShell на комп'ютері, де відбувається аварійне завершення роботи, і виконайте такі команди:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Вкладіть файл у свій інцидент служби підтримки.
