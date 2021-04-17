---
title: Усунення несправностей, пов'язаних із аварійно заверш
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
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826220"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="70bf8-102">Усунення несправностей, пов'язаних із аварійно заверш</span><span class="sxs-lookup"><span data-stu-id="70bf8-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="70bf8-103">Якщо OneDrive неодноразово аварійно завершує роботу, спробуйте виконати наведені нижче дії з виправлення неполадок.</span><span class="sxs-lookup"><span data-stu-id="70bf8-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="70bf8-104">**Переконайтеся, що розділи реєстру не настроєно.**</span><span class="sxs-lookup"><span data-stu-id="70bf8-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="70bf8-105">За допомогою редактора реєстру перейдіть до HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="70bf8-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="70bf8-106">Якщо disableFileSyncNGSC встановлено та встановлено значення 1, відкрийте ключ і змініть значення на 0.</span><span class="sxs-lookup"><span data-stu-id="70bf8-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="70bf8-107">Вручну запустіть OneDrive у меню "Пуск"</span><span class="sxs-lookup"><span data-stu-id="70bf8-107">Manually launch OneDrive by going to Start</span></span> ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="70bf8-109">, введіть OneDrive у полі пошуку, а потім клацніть класичну програму OneDrive.</span><span class="sxs-lookup"><span data-stu-id="70bf8-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="70bf8-110">**Скидання OneDrive**</span><span class="sxs-lookup"><span data-stu-id="70bf8-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="70bf8-111">Примітки.</span><span class="sxs-lookup"><span data-stu-id="70bf8-111">Notes:</span></span>

- <span data-ttu-id="70bf8-112">Під час скидання OneDrive роз'єднує всі наявні підключення для синхронізації (включно з особистим обліковим записом OneDrive, якщо його налаштовано).</span><span class="sxs-lookup"><span data-stu-id="70bf8-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="70bf8-113">Ви не втратите файли або дані, якщо скинете параметри OneDrive на комп'ютері.</span><span class="sxs-lookup"><span data-stu-id="70bf8-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="70bf8-114">**Щоб скинути параметри OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="70bf8-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="70bf8-115">Відкрийте діалогове вікно "Виконати", натиснувши клавіші Windows і R.</span><span class="sxs-lookup"><span data-stu-id="70bf8-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="70bf8-116">Введіть %localappdata%\Microsoft\OneDrive\onedrive.exe /reset і натисніть кнопку OK.</span><span class="sxs-lookup"><span data-stu-id="70bf8-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="70bf8-117">Коротко може з'явитися вікно командного рядка.</span><span class="sxs-lookup"><span data-stu-id="70bf8-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="70bf8-118">Вручну запустіть OneDrive у меню "Пуск"</span><span class="sxs-lookup"><span data-stu-id="70bf8-118">Manually launch OneDrive by going to Start</span></span> ![Натисніть клавішу Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="70bf8-120">, введіть OneDrive у полі пошуку, а потім клацніть класичну програму OneDrive.</span><span class="sxs-lookup"><span data-stu-id="70bf8-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="70bf8-121">Примітки.</span><span class="sxs-lookup"><span data-stu-id="70bf8-121">Notes:</span></span>

- <span data-ttu-id="70bf8-122">Якщо ви синхронізувати лише певні папки до скидання, це потрібно зробити ще раз після синхронізації.</span><span class="sxs-lookup"><span data-stu-id="70bf8-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="70bf8-123">Докладні відомості див. в розділі Вибір папок [OneDrive, які потрібно синхронізувати з](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   комп'ютером.</span><span class="sxs-lookup"><span data-stu-id="70bf8-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="70bf8-124">Це потрібно зробити для особистого сховища OneDrive і "OneDrive для бізнесу".</span><span class="sxs-lookup"><span data-stu-id="70bf8-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>