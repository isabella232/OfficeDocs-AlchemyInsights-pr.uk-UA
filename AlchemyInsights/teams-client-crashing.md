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
# <a name="teams-client-crashing"></a><span data-ttu-id="ffe7b-102">Teams аварійне завершення роботи клієнта</span><span class="sxs-lookup"><span data-stu-id="ffe7b-102">Teams client crashing</span></span>

<span data-ttu-id="ffe7b-103">Якщо клієнт Teams аварійно завершує роботу, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="ffe7b-104">Якщо ви використовуєте класичну версію програми Teams, [переконайтеся, що її повністю оновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="ffe7b-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="ffe7b-105">Переконайтеся, що [всі Microsoft 365 URL-адреси та діапазони](/microsoftteams/connectivity-issues) адрес доступні.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="ffe7b-106">Увійдіть під обліковим записом адміністратора клієнта та перевірте приладну дошку справності служби, щоб переконатися, що немає перебоїв або погіршення якості служби. [](/office365/enterprise/view-service-health)</span><span class="sxs-lookup"><span data-stu-id="ffe7b-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="ffe7b-107">Видалення та повторна Teams програми</span><span class="sxs-lookup"><span data-stu-id="ffe7b-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="ffe7b-108">Перейдіть до папки %appdata%\Microsoft\Teams\ на комп'ютері та видаліть усі файли з цього каталогу.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="ffe7b-109">[Завантажте та інсталюйте програму Teams](https://www.microsoft.com/microsoft-teams/download-app)і, за можливості, інсталюйте Teams як адміністратор (клацніть правою кнопкою миші інсталятор Teams і виберіть команду Запустити із правами адміністратора, якщо він доступний). </span><span class="sxs-lookup"><span data-stu-id="ffe7b-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="ffe7b-110">Якщо клієнт Teams аварійно завершує роботу, спробуйте відтворити проблему.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="ffe7b-111">У такому разі ви зможете:</span><span class="sxs-lookup"><span data-stu-id="ffe7b-111">If you can:</span></span>

1. <span data-ttu-id="ffe7b-112">Щоб записати кроки, скористайтеся записуванням дій.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="ffe7b-113">Закрийте всі непотрібні або конфіденційні програми.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="ffe7b-114">Запустіть записувач кроків і відтворіть цю проблему під час входу за допомогою відповідного облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="ffe7b-115">[Зберіть журнали команд, у яких записано кроки повторного відтворення.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="ffe7b-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="ffe7b-116">**Примітка.** Обов'язково запишіть адресу для входу потрібного користувача.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="ffe7b-117">Зберіть дамп і/або відомості про блок Windows.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="ffe7b-118">Запустіть Windows powershell на комп'ютері, де відбувається аварійне завершення роботи, і виконайте наведені нижче команди (після кожної команди натисніть клавішу Enter):</span><span class="sxs-lookup"><span data-stu-id="ffe7b-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="ffe7b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="ffe7b-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="ffe7b-120">Створиться текстовий файл, який з'явиться на екрані, збережіть файл і вкладіть його в запит на обслуговування.</span><span class="sxs-lookup"><span data-stu-id="ffe7b-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
