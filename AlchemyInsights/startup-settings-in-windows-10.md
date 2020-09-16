---
title: Параметри запуску в ОС Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751156"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="a8262-102">Параметри запуску в ОС Windows 10</span><span class="sxs-lookup"><span data-stu-id="a8262-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="a8262-103">**Змінення програм, які запускаються автоматично під час запуску**</span><span class="sxs-lookup"><span data-stu-id="a8262-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="a8262-104">Виберіть [настройки > програм > запуску](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="a8262-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="a8262-105">Переконайтеся, що всі програми, які потрібно запустити під час запуску, **увімкнуто.**</span><span class="sxs-lookup"><span data-stu-id="a8262-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="a8262-106">**Додавання програми для автоматичного запуску під час запуску**</span><span class="sxs-lookup"><span data-stu-id="a8262-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="a8262-107">Натисніть кнопку **Пуск** і виберіть програму, яку потрібно запустити під час запуску.</span><span class="sxs-lookup"><span data-stu-id="a8262-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="a8262-108">Клацніть програму правою кнопкою миші, виберіть пункт **Додатково**, а потім виберіть пункт **відкрити розташування файлу**.</span><span class="sxs-lookup"><span data-stu-id="a8262-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="a8262-109">Відкриється місце, де буде збережено ярлик для програми.</span><span class="sxs-lookup"><span data-stu-id="a8262-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="a8262-110">Якщо не вдається відкрити розташування файлу, це означає, що програма не може виконуватися під час запуску.</span><span class="sxs-lookup"><span data-stu-id="a8262-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="a8262-111">Відкривши розташування файлу, натисніть клавішу з **емблемою Windows + R**, введіть **оболонку: запуск**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8262-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="a8262-112">Відкриється папка автозавантаження.</span><span class="sxs-lookup"><span data-stu-id="a8262-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="a8262-113">Скопіюйте та вставте ярлик у програму з розташування файлу до папки автозавантаження.</span><span class="sxs-lookup"><span data-stu-id="a8262-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="a8262-114">**Додаткові параметри запуску (зокрема безпечний режим, настройки UEFI та завантаження з іншого пристрою)**</span><span class="sxs-lookup"><span data-stu-id="a8262-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="a8262-115">Збережіть роботу та закрийте всі відкриті документи, оскільки ці кроки буде перезавантажено на ПК.</span><span class="sxs-lookup"><span data-stu-id="a8262-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="a8262-116">Перейдіть до розділу [настройки > оновити & безпека > відновлення](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="a8262-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="a8262-117">У розділі **Розширений запуск**натисніть кнопку **Перезавантажити зараз**.</span><span class="sxs-lookup"><span data-stu-id="a8262-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="a8262-118">Після перезавантаження ПК на екрані Вибір параметра виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="a8262-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="a8262-119">Щоб завантажитися з пристрою, як-от USB-накопичувач, натисніть кнопку **використовувати пристрій**.</span><span class="sxs-lookup"><span data-stu-id="a8262-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="a8262-120">Щоб перейти до настройок UEFI (іноді її називають "Настроювання BIOS"), натисніть кнопку **усунути неполадки > розширені параметри > настройки прошивки UEFI**.</span><span class="sxs-lookup"><span data-stu-id="a8262-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="a8262-121">Щоб перейти в безпечний режим або змінити розширені настройки запуску, клацніть **Виправлення неполадок > розширені параметри > настройки запуску**, а потім натисніть кнопку **перезапустити**.</span><span class="sxs-lookup"><span data-stu-id="a8262-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="a8262-122">Можливо, вам буде запропоновано ввести [ключ відновлення BitLocker](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="a8262-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="a8262-123">Після повторного перезавантаження ПК клацніть настройку запуску, яку потрібно використовувати.</span><span class="sxs-lookup"><span data-stu-id="a8262-123">After your PC restarts again, click the startup setting you want to use.</span></span>