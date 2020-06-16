---
title: Усунення несправностей OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749241"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="7929a-102">Усунення несправностей OneDrive</span><span class="sxs-lookup"><span data-stu-id="7929a-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="7929a-103">Якщо OneDrive кілька разів аварійно завершує роботу, спробуйте виконати такі дії:</span><span class="sxs-lookup"><span data-stu-id="7929a-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="7929a-104">**Переконайтеся, що розділи реєстру не встановлено:**</span><span class="sxs-lookup"><span data-stu-id="7929a-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="7929a-105">За допомогою редактора реєстру, перейдіть до HKEY_LOCAL_MACHINE \ програмне забезпечення\price\micti</span><span class="sxs-lookup"><span data-stu-id="7929a-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="7929a-106">Якщо в наявності є 1, відкрийте ключ і змініть значення на 0, якщо він є.</span><span class="sxs-lookup"><span data-stu-id="7929a-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="7929a-107">Запустіть OneDrive вручну, перейшовши на початок</span><span class="sxs-lookup"><span data-stu-id="7929a-107">Manually launch OneDrive by going to Start</span></span> ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="7929a-109">, у полі пошуку введіть OneDrive, а потім клацніть програму OneDrive для настільних комп'ютерів.</span><span class="sxs-lookup"><span data-stu-id="7929a-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="7929a-110">**Скинути OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="7929a-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="7929a-111">Нотатки:</span><span class="sxs-lookup"><span data-stu-id="7929a-111">Notes:</span></span>

- <span data-ttu-id="7929a-112">Скидання настройок OneDrive припиняється з усіма існуючими синхронізованими підключеннями (включно з особистими OneDrive у разі настроювання).</span><span class="sxs-lookup"><span data-stu-id="7929a-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="7929a-113">Ви не втратите файли або дані, відновивши OneDrive на комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="7929a-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="7929a-114">**Щоб скинути OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="7929a-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="7929a-115">Щоб відкрити діалогове вікно запуску, натисніть клавішу Windows і R.</span><span class="sxs-lookup"><span data-stu-id="7929a-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="7929a-116">Введіть% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset і натисніть OK.</span><span class="sxs-lookup"><span data-stu-id="7929a-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="7929a-117">Вікно командного рядка може здатися коротко.</span><span class="sxs-lookup"><span data-stu-id="7929a-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="7929a-118">Запустіть OneDrive вручну, перейшовши на початок</span><span class="sxs-lookup"><span data-stu-id="7929a-118">Manually launch OneDrive by going to Start</span></span> ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="7929a-120">, у полі пошуку введіть OneDrive, а потім клацніть програму OneDrive для настільних комп'ютерів.</span><span class="sxs-lookup"><span data-stu-id="7929a-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="7929a-121">Нотатки:</span><span class="sxs-lookup"><span data-stu-id="7929a-121">Notes:</span></span>

- <span data-ttu-id="7929a-122">Якщо ви вирішили синхронізувати лише деякі папки перед скиданням, вам потрібно буде зробити це знову після завершення синхронізації.</span><span class="sxs-lookup"><span data-stu-id="7929a-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="7929a-123">Дізнайтеся [, як вибрати папки OneDrive для синхронізації з комп'ютером](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   для отримання додаткових відомостей.</span><span class="sxs-lookup"><span data-stu-id="7929a-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="7929a-124">Вам потрібно буде завершити це для вашого особистого OneDrive і OneDrive для бізнесу.</span><span class="sxs-lookup"><span data-stu-id="7929a-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>