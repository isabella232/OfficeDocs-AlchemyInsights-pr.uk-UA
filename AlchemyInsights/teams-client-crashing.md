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
# <a name="teams-client-crashing"></a><span data-ttu-id="a93c8-102">Клієнт Teams аварійно завершує роботу?</span><span class="sxs-lookup"><span data-stu-id="a93c8-102">Teams client crashing?</span></span>

<span data-ttu-id="a93c8-103">Якщо клієнт Teams аварійно завершує роботу, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="a93c8-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a93c8-104">Якщо ви використовуєте класичну версію програми Teams, [переконайтеся, що її повністю оновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a93c8-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a93c8-105">Переконайтеся, що всі [URL-адреси Microsoft 365 і діапазони адрес](https://docs.microsoft.com/microsoftteams/connectivity-issues) доступні.</span><span class="sxs-lookup"><span data-stu-id="a93c8-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a93c8-106">Увійдіть у систему з обліковим записом адміністратора клієнта та перевірте [приладну дошку справності](https://docs.microsoft.com/office365/enterprise/view-service-health) , щоб перевірити, чи існує відсутність перебої або погіршення служби.</span><span class="sxs-lookup"><span data-stu-id="a93c8-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="a93c8-107">Видаліть і переінсталюйте програму teams (посилання)</span><span class="sxs-lookup"><span data-stu-id="a93c8-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="a93c8-108">Перейдіть до%Appded%\mice\systems\ папки на комп'ютері та видалити всі файли в цьому каталозі.</span><span class="sxs-lookup"><span data-stu-id="a93c8-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="a93c8-109">[Скачайте і встановіть додаток teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), і, якщо можливо, встановіть teams як адміністратор (клацніть правою кнопкою миші інсталятор команд і виберіть "Запуск від як адміністратор", якщо доступно).</span><span class="sxs-lookup"><span data-stu-id="a93c8-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="a93c8-110">Якщо ваш клієнт команди все ще збій, ви можете відтворити проблему?</span><span class="sxs-lookup"><span data-stu-id="a93c8-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="a93c8-111">Якщо так:</span><span class="sxs-lookup"><span data-stu-id="a93c8-111">If so:</span></span>

1. <span data-ttu-id="a93c8-112">Використовуйте засіб записування дій, щоб захопити ваші дії.</span><span class="sxs-lookup"><span data-stu-id="a93c8-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="a93c8-113">Закрийте всі непотрібні або конфіденційні програми.</span><span class="sxs-lookup"><span data-stu-id="a93c8-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="a93c8-114">Запустіть засіб записування дій і відтворити проблему, під час входу з відповідного облікового запису користувача.</span><span class="sxs-lookup"><span data-stu-id="a93c8-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="a93c8-115">[Зберіть команди журналів, які захоплюють записані відтворення зв кроки](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="a93c8-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="a93c8-116">**Зверніть увагу**: переконайтеся, що ви захоплення входу адресу впливу користувача.</span><span class="sxs-lookup"><span data-stu-id="a93c8-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="a93c8-117">Збір дампа і/або несправність інформації відро (Windows).</span><span class="sxs-lookup"><span data-stu-id="a93c8-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="a93c8-118">Запустіть Windows PowerShell на комп'ютері, де відбувається збій і виконайте такі команди:</span><span class="sxs-lookup"><span data-stu-id="a93c8-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="a93c8-119">Прикріпіть файл до справи підтримки.</span><span class="sxs-lookup"><span data-stu-id="a93c8-119">Attach the file to your support case.</span></span>
