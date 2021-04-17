---
title: Параметри запуску у Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828173"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="30716-102">Параметри запуску у Windows 10</span><span class="sxs-lookup"><span data-stu-id="30716-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="30716-103">**Змінення програм, які запускаються автоматично під час запуску системи**</span><span class="sxs-lookup"><span data-stu-id="30716-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="30716-104">Виберіть елементи [Настройки > Програми > запуск.](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="30716-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="30716-105">Переконайтеся, що будь-яку програму, яку потрібно запускати під час запуску, увімкнуто .</span><span class="sxs-lookup"><span data-stu-id="30716-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="30716-106">**Додавання програми для автоматичного запуску**</span><span class="sxs-lookup"><span data-stu-id="30716-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="30716-107">Натисніть кнопку **Пуск** і знайдіть програму, яку потрібно запустити під час запуску.</span><span class="sxs-lookup"><span data-stu-id="30716-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="30716-108">Клацніть програму правою кнопкою миші, виберіть пункт **Додатково**, а потім виберіть **пункт Відкрити розташування файлу.**</span><span class="sxs-lookup"><span data-stu-id="30716-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="30716-109">Відкриється розташування, у якому збережено ярлик програми.</span><span class="sxs-lookup"><span data-stu-id="30716-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="30716-110">Якщо для параметра "Відкрити розташування файлу" немає параметра, це означає, що програма не може запуститися під час запуску.</span><span class="sxs-lookup"><span data-stu-id="30716-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="30716-111">Відкрийте файл у розташуванні, натисніть **клавіші Windows+R,** введіть **shell:startup**, а потім натисніть кнопку **OK.**</span><span class="sxs-lookup"><span data-stu-id="30716-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="30716-112">Відкриється папка автозавантаження.</span><span class="sxs-lookup"><span data-stu-id="30716-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="30716-113">Скопіюйте та вставте ярлик програми з розташування файлу до папки автозавантаження.</span><span class="sxs-lookup"><span data-stu-id="30716-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="30716-114">**Додаткові параметри запуску (зокрема безпечний режим, настройки UEFI та завантаження з іншого пристрою)**</span><span class="sxs-lookup"><span data-stu-id="30716-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="30716-115">Збережіть свою роботу та закрийте всі відкриті документи, оскільки ці дії перезавантажать комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="30716-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="30716-116">Послідовно [виберіть елементи Настройки > Оновлення & безпеки > відновлення.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="30716-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="30716-117">У розділі **Додаткові параметри запуску натисніть** кнопку **Перезавантажити зараз.**</span><span class="sxs-lookup"><span data-stu-id="30716-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="30716-118">Коли ПК перезавантажиться, на екрані Виберіть варіант:</span><span class="sxs-lookup"><span data-stu-id="30716-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="30716-119">Щоб завантажити його з пристрою, наприклад USB-носія, натисніть **кнопку "Використовувати пристрій".**</span><span class="sxs-lookup"><span data-stu-id="30716-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="30716-120">Щоб ввести параметри UEFI (інколи називається налаштуванням BIOS), виберіть посилання > додаткові параметри > мікропрограми **UEFI.**</span><span class="sxs-lookup"><span data-stu-id="30716-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="30716-121">Щоб увійти в безпечний режим або змінити додаткові параметри запуску, клацніть Виправлення неполадок **> додаткових параметрів >** параметрах запуску та натисніть кнопку Перезавантажити . </span><span class="sxs-lookup"><span data-stu-id="30716-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="30716-122">Можливо, знадобиться ввести [ключ відновлення BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="30716-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="30716-123">Коли ПК знову перезавантажиться, клацніть потрібну настройку запуску.</span><span class="sxs-lookup"><span data-stu-id="30716-123">After your PC restarts again, click the startup setting you want to use.</span></span>