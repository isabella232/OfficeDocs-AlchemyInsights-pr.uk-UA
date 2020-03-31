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
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030759"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="cb6ee-102">Клієнт Teams аварійно завершує роботу?</span><span class="sxs-lookup"><span data-stu-id="cb6ee-102">Teams client crashing?</span></span>

<span data-ttu-id="cb6ee-103">Якщо клієнт Teams аварійно завершує роботу, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="cb6ee-104">Якщо ви використовуєте класичну версію програми Teams, [переконайтеся, що її повністю оновлено](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="cb6ee-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="cb6ee-105">Переконайтеся, що всі [діапазони URL- і IP-адрес Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) доступні.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="cb6ee-106">Увійдіть за допомогою облікового запису адміністратора та перегляньте [приладну дошку стану служби](https://docs.microsoft.com/office365/enterprise/view-service-health), щоб переконатись у відсутності перебоїв у роботі та зменшення продуктивності служби.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="cb6ee-107">На останньому кроці ви можете спробувати очистити кеш клієнта Teams.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="cb6ee-108">Повністю вийдіть із класичної програми Microsoft Team.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="cb6ee-109">Клацніть правою кнопкою миші **Teams** на піктограмі в системній треї, а потім виберіть **Вийти**. Ви також можете запустити диспетчер завдань і повністю вимкнути процес.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="cb6ee-110">Відкрийте Файловий провідник і введіть %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="cb6ee-111">У каталозі з’являться кілька наведених нижче папок.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="cb6ee-112">Виберіть **Application Cache**, відкрийте папку Cache і видаліть із неї всі файли: %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="cb6ee-113">З папки **Blob_storage** видаліть усі файли: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="cb6ee-114">З папки **Cache** видаліть усі файли: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="cb6ee-115">З папки **databases** видаліть усі файли: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="cb6ee-116">З папки **GPUCache** видаліть усі файли: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="cb6ee-117">З папки **IndexedDB** видаліть DB-файл: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="cb6ee-118">З папки **Local Storage** видаліть усі файли: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="cb6ee-119">Насамкінець із папки **tmp** видаліть усі файли: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="cb6ee-120">Перезапустіть клієнт Teams.</span><span class="sxs-lookup"><span data-stu-id="cb6ee-120">Restart your Teams client.</span></span>
