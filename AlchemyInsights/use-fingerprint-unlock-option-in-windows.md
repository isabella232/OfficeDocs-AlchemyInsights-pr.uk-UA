---
title: Використання параметра розблокування відбитків пальців у Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588336"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="bf59b-102">Використання параметра розблокування відбитків пальців у Windows 10</span><span class="sxs-lookup"><span data-stu-id="bf59b-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="bf59b-103">**Увімкнути відбиток пальця Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="bf59b-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="bf59b-104">Щоб розблокувати Windows 10 за допомогою відбитків пальців, потрібно настроїти відбиток пальця Windows Hello за допомогою додавання (дозволити Windows навчитися розпізнавати) принаймні один палець.</span><span class="sxs-lookup"><span data-stu-id="bf59b-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="bf59b-105">Перейдіть до **налаштувань > облікових записів > Параметри входу** (або натисніть [тут](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="bf59b-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="bf59b-106">Доступні Параметри входу будуть перераховані.</span><span class="sxs-lookup"><span data-stu-id="bf59b-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="bf59b-107">Наприклад,</span><span class="sxs-lookup"><span data-stu-id="bf59b-107">For example:</span></span>

    ![Параметри входу.](media/sign-in-options.png)

2. <span data-ttu-id="bf59b-109">Клацніть або торкніться **відбитків пальців Windows Hello**, а потім натисніть кнопку **настроїти**.</span><span class="sxs-lookup"><span data-stu-id="bf59b-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="bf59b-110">У вікні Настроювання Windows **Hello натисніть кнопку почати.**</span><span class="sxs-lookup"><span data-stu-id="bf59b-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="bf59b-111">Буде активовано датчик відбитків пальців, і вам буде запропоновано помістити палець на датчик:</span><span class="sxs-lookup"><span data-stu-id="bf59b-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Датчик відбитків пальців.](media/fingerprint-sensor.png)

3. <span data-ttu-id="bf59b-113">Дотримуйтесь інструкцій, які будуть просити вас повторно сканувати палець.</span><span class="sxs-lookup"><span data-stu-id="bf59b-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="bf59b-114">Коли це буде закінчено, ви матимете можливість додати інші пальці, які ви можете використовувати для входу.</span><span class="sxs-lookup"><span data-stu-id="bf59b-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="bf59b-115">Наступного разу, коли ви входите у Windows 10, ви будете мати можливість використовувати відбиток пальця, щоб зробити це.</span><span class="sxs-lookup"><span data-stu-id="bf59b-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="bf59b-116">**Відбиток пальця Windows Hello недоступний як параметр входу**</span><span class="sxs-lookup"><span data-stu-id="bf59b-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="bf59b-117">Якщо в **параметрах входу**немає функції відбитків пальців Windows Hello, це означає, що Windows не відомо про будь-який сканер відбитків пальців або сканера, ПІДКЛЮЧЕНИЙ до ПК, або що системна політика запобігає його використанню (якщо, наприклад, ваш ПК керує вашим робочим місцем).</span><span class="sxs-lookup"><span data-stu-id="bf59b-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="bf59b-118">Щоб усунути неполадки:</span><span class="sxs-lookup"><span data-stu-id="bf59b-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="bf59b-119">Натисніть кнопку **Пуск** на панелі завдань і знайдіть **Диспетчер пристроїв**.</span><span class="sxs-lookup"><span data-stu-id="bf59b-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="bf59b-120">Клацніть або торкніться, щоб відкрити **Диспетчер пристроїв**.</span><span class="sxs-lookup"><span data-stu-id="bf59b-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="bf59b-121">У диспетчері пристроїв розгорніть вузол Біометричні пристрої, клацнувши його Шеврон.</span><span class="sxs-lookup"><span data-stu-id="bf59b-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Біометричні пристрої.](media/biometric-devices.png)

4. <span data-ttu-id="bf59b-123">Сканер відбитків пальців повинен бути вказаний як біометричний пристрій, наприклад Synaptics WBDI Scanner:</span><span class="sxs-lookup"><span data-stu-id="bf59b-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Біометричні пристрої.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="bf59b-125">Якщо сканер відбитків пальців не відображається, а сканер інтегрований у ваш ПК, перейдіть на веб-сайт виробника комп'ютера.</span><span class="sxs-lookup"><span data-stu-id="bf59b-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="bf59b-126">У розділі технічної підтримки для моделі ПК знайдіть драйвер Windows 10 для сканера, який можна інсталювати.</span><span class="sxs-lookup"><span data-stu-id="bf59b-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="bf59b-127">Якщо сканер відділено від ПК (додається через USB), перейдіть на веб-сайт виробника сканера, щоб знайти та інсталювати програмне забезпечення драйвера пристрою Windows 10 для моделі сканера.</span><span class="sxs-lookup"><span data-stu-id="bf59b-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
