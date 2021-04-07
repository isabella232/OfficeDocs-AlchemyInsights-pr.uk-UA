---
title: Вивільнення простору у Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505377"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="174b2-102">Вивільнення простору у Windows 10</span><span class="sxs-lookup"><span data-stu-id="174b2-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="174b2-103">Ось два способи вивільнити простір на диску у Windows:</span><span class="sxs-lookup"><span data-stu-id="174b2-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="174b2-104">Вивільнення простору у Windows 10.</span><span class="sxs-lookup"><span data-stu-id="174b2-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="174b2-105">Вивільніть простір для оновлень Windows 10 за допомогою зовнішнього накопичувача.</span><span class="sxs-lookup"><span data-stu-id="174b2-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="174b2-106">Якщо після використання програми очищення диска простору все одно бракує, можливо, папка "Temp" швидко заповнюється файлами програм (APPX), які використовуються в Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="174b2-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="174b2-107">Щоб усунути цю проблему, скиньте Microsoft Store, очистьте кеш цієї служби, а потім запустіть засіб усунення неполадок Windows Update.</span><span class="sxs-lookup"><span data-stu-id="174b2-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="174b2-108">Перш ніж виконати ці дії, обов’язково закрийте Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="174b2-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="174b2-109">**Крок 1: скиньте Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="174b2-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="174b2-110">**Примітка.** Ця дія остаточно видаляє дані програм на пристрої, зокрема параметри та відомості для входу.</span><span class="sxs-lookup"><span data-stu-id="174b2-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="174b2-111">Виберіть **Пуск** > **Настройки** > **Програми** > **Програми та функції**.</span><span class="sxs-lookup"><span data-stu-id="174b2-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="174b2-112">У списку програм знайдіть і виберіть Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="174b2-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="174b2-113">Виберіть **Додаткові параметри**.</span><span class="sxs-lookup"><span data-stu-id="174b2-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="174b2-114">Прокрутіть униз і виберіть **Скинути**, а потім — **Підтвердити скидання**.</span><span class="sxs-lookup"><span data-stu-id="174b2-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="174b2-115">**Крок 2: очистьте кеш Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="174b2-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="174b2-116">Натисніть Windows+R, щоб відкрити діалогове вікно "Виконати".</span><span class="sxs-lookup"><span data-stu-id="174b2-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="174b2-117">Введіть wsreset.exe і виберіть **OK**.</span><span class="sxs-lookup"><span data-stu-id="174b2-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="174b2-118">Відкриється вікно пустого командного рядка.</span><span class="sxs-lookup"><span data-stu-id="174b2-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="174b2-119">Приблизно через 10 секунд вікно закриється, а Microsoft Store відкриється.</span><span class="sxs-lookup"><span data-stu-id="174b2-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="174b2-120">**Крок 3: скиньте Windows Update**</span><span class="sxs-lookup"><span data-stu-id="174b2-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="174b2-121">Виберіть **Пуск** > **Настройки** > **Оновлення та захист** > **Виправити неполадки**.</span><span class="sxs-lookup"><span data-stu-id="174b2-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="174b2-122">Прокрутіть униз і виберіть **Windows Update** у списку, а потім – **Запустити засіб усунення неполадок**.</span><span class="sxs-lookup"><span data-stu-id="174b2-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="174b2-123">Перезавантажте комп’ютер і перевірте, чи проблема досі наявна.</span><span class="sxs-lookup"><span data-stu-id="174b2-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

