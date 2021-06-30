---
title: Teams аварійне завершення роботи клієнта
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187742"
---
# <a name="teams-client-crashing"></a>Teams аварійне завершення роботи клієнта

Якщо клієнт Teams аварійно завершує роботу, виконайте наведені нижче дії.

- Якщо ви використовуєте класичну версію програми Teams, [переконайтеся, що її повністю оновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Переконайтеся, що [всі Microsoft 365 URL-адреси та діапазони](/microsoftteams/connectivity-issues) адрес доступні.

- Увійдіть під обліковим записом адміністратора клієнта та перевірте приладну дошку справності служби, щоб переконатися, що немає перебоїв або погіршення якості служби. [](/office365/enterprise/view-service-health)

- Видалення та повторна Teams програми
    - Перейдіть до папки %appdata%\Microsoft\Teams\ на комп'ютері та видаліть усі файли з цього каталогу.
    - [Завантажте та інсталюйте програму Teams](https://www.microsoft.com/microsoft-teams/download-app)і, за можливості, інсталюйте Teams як адміністратор (клацніть правою кнопкою миші інсталятор Teams і виберіть команду Запустити із правами адміністратора, якщо він доступний). 

Якщо клієнт Teams аварійно завершує роботу, спробуйте відтворити проблему. У такому разі ви зможете:

1. Щоб записати кроки, скористайтеся записуванням дій.
    - Закрийте всі непотрібні або конфіденційні програми.
    - Запустіть записувач кроків і відтворіть цю проблему під час входу за допомогою відповідного облікового запису користувача.
    - [Зберіть журнали команд, у яких записано кроки повторного відтворення.](/microsoftteams/log-files) **Примітка.** Обов'язково запишіть адресу для входу потрібного користувача.
    - Зберіть дамп і/або відомості про блок Windows. Запустіть Windows powershell на комп'ютері, де відбувається аварійне завершення роботи, і виконайте наведені нижче команди (після кожної команди натисніть клавішу Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Створиться текстовий файл, який з'явиться на екрані, збережіть файл і вкладіть його в запит на обслуговування. 
