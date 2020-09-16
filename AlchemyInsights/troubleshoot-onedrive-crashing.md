---
title: Усунення несправностей у OneDrive
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665019"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="f900a-102">Усунення несправностей у OneDrive</span><span class="sxs-lookup"><span data-stu-id="f900a-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="f900a-103">Якщо не вдається повторно завершити роботу, виконайте наведені нижче дії з виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="f900a-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="f900a-104">**Переконайтеся, що розділи реєстру не настроєно:**</span><span class="sxs-lookup"><span data-stu-id="f900a-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="f900a-105">У редакторі реєстру перейдіть до HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="f900a-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="f900a-106">Якщо DisableFileSyncNGSC присутній і настроєно на 1, відкрийте ключ і змініть значення на 0.</span><span class="sxs-lookup"><span data-stu-id="f900a-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="f900a-107">Запуск OneDrive вручну за допомогою переходу на початок</span><span class="sxs-lookup"><span data-stu-id="f900a-107">Manually launch OneDrive by going to Start</span></span> ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f900a-109">, у полі пошуку введіть OneDrive, а потім клацніть піктограму для настільних комп'ютерів у програмі OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f900a-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f900a-110">**Скидання "OneDrive":**</span><span class="sxs-lookup"><span data-stu-id="f900a-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="f900a-111">Нотаток</span><span class="sxs-lookup"><span data-stu-id="f900a-111">Notes:</span></span>

- <span data-ttu-id="f900a-112">Скидання "OneDrive" відключає всі поточні зв'язки синхронізації (включно з особистим "OneDrive", якщо його настроєно).</span><span class="sxs-lookup"><span data-stu-id="f900a-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="f900a-113">Ви не втратите файли або дані, скинувши OneDrive на вашому комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="f900a-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="f900a-114">**Щоб скинути його, виконайте наведені нижче дії.**</span><span class="sxs-lookup"><span data-stu-id="f900a-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="f900a-115">Відкрийте діалогове вікно "виконати", натиснувши клавіші Windows і R.</span><span class="sxs-lookup"><span data-stu-id="f900a-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="f900a-116">Введіть% localappdata% \Microsoft\OneDrive\onedrive.exe/Reset. і натисніть кнопку OK.</span><span class="sxs-lookup"><span data-stu-id="f900a-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="f900a-117">У вікні командного рядка може відображатися короткий час.</span><span class="sxs-lookup"><span data-stu-id="f900a-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="f900a-118">Запуск OneDrive вручну за допомогою переходу на початок</span><span class="sxs-lookup"><span data-stu-id="f900a-118">Manually launch OneDrive by going to Start</span></span> ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="f900a-120">, у полі пошуку введіть OneDrive, а потім клацніть піктограму для настільних комп'ютерів у програмі OneDrive.</span><span class="sxs-lookup"><span data-stu-id="f900a-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="f900a-121">Нотаток</span><span class="sxs-lookup"><span data-stu-id="f900a-121">Notes:</span></span>

- <span data-ttu-id="f900a-122">Якщо ви вирішили синхронізувати лише деякі папки перед скиванням, потрібно буде виконати цю дію знову після завершення синхронізації.</span><span class="sxs-lookup"><span data-stu-id="f900a-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="f900a-123">Дізнайтеся [, які папки OneDrive синхронізуються з комп'ютером,](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)щоб отримати   докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="f900a-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="f900a-124">Вам потрібно буде виконати це для особистого "OneDrive" та "OneDrive для бізнесу".</span><span class="sxs-lookup"><span data-stu-id="f900a-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>