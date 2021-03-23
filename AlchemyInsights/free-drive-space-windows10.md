---
title: Звільніть місце на диску в ОС Windows 10
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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037953"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="d9258-102">Звільніть місце на диску в ОС Windows 10</span><span class="sxs-lookup"><span data-stu-id="d9258-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="d9258-103">Нижче наведено два способи звільнити місце на диску в ОС Windows.</span><span class="sxs-lookup"><span data-stu-id="d9258-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="d9258-104">Звільніть місце на диску в операційній системі Windows 10.</span><span class="sxs-lookup"><span data-stu-id="d9258-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="d9258-105">Звільніть місце для оновлень Windows 10 із зовнішнім пристроєм збереження даних.</span><span class="sxs-lookup"><span data-stu-id="d9258-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="d9258-106">Якщо після використання засобу очищення диска все ще бракує вільного дискового простору, можливо, ваша папка Temp швидко заповнює файли застосунків (. Appx), які використовуються в Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="d9258-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="d9258-107">Щоб вирішити цю проблему, скиньте магазин, очистьте кеш магазину, а потім запустіть засіб усунення неполадок Windows Update.</span><span class="sxs-lookup"><span data-stu-id="d9258-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="d9258-108">Переконайтеся, що програму Microsoft Store закрито, перш ніж продовжити ці дії.</span><span class="sxs-lookup"><span data-stu-id="d9258-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="d9258-109">**Крок 1: скидання Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="d9258-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="d9258-110">**Примітка** . Після цього остаточно видаляються дані програми на пристрої, включно з вашими параметрами та відомостями про вхід.</span><span class="sxs-lookup"><span data-stu-id="d9258-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="d9258-111">Натисніть кнопку " **розпочати** налаштування програм програм"  >    >    >  **& функцій**.</span><span class="sxs-lookup"><span data-stu-id="d9258-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="d9258-112">У списку програм знайдіть і виберіть пункт Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="d9258-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="d9258-113">Виберіть **Додаткові параметри**.</span><span class="sxs-lookup"><span data-stu-id="d9258-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="d9258-114">Прокрутіть униз і натисніть кнопку **скинути**, а потім **підтвердьте скидання**.</span><span class="sxs-lookup"><span data-stu-id="d9258-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="d9258-115">**Крок 2: очищення кеша магазину Microsoft**</span><span class="sxs-lookup"><span data-stu-id="d9258-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="d9258-116">Натисніть клавішу з емблемою Windows + R, щоб відкрити діалогове вікно виконати.</span><span class="sxs-lookup"><span data-stu-id="d9258-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="d9258-117">Введіть wsreset.exe та натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="d9258-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="d9258-118">Відкриється вікно "пустий командний рядок".</span><span class="sxs-lookup"><span data-stu-id="d9258-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="d9258-119">Після 10 секунд вікно закриється, і магазин відкриється автоматично.</span><span class="sxs-lookup"><span data-stu-id="d9258-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="d9258-120">**Крок 3: скидання Windows Update**</span><span class="sxs-lookup"><span data-stu-id="d9258-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="d9258-121">Виберіть елемент **почати**  >    >  **оновлення &**  >  **Виправлення неполадок** системи безпеки.</span><span class="sxs-lookup"><span data-stu-id="d9258-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="d9258-122">Прокрутіть униз і виберіть пункт **Windows Update** зі списку, а потім виберіть команду **запустити засіб усунення неполадок**.</span><span class="sxs-lookup"><span data-stu-id="d9258-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="d9258-123">Перезавантажте комп'ютер і перевірте, чи все ще виникає проблема.</span><span class="sxs-lookup"><span data-stu-id="d9258-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

