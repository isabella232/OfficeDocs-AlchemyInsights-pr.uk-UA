---
title: Використання параметра розблокування відбитків пальців у Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796698"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="14bc1-102">Використання параметра розблокування відбитків пальців у Windows 10</span><span class="sxs-lookup"><span data-stu-id="14bc1-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="14bc1-103">**Увімкнення відбитків пальців Windows Hello**</span><span class="sxs-lookup"><span data-stu-id="14bc1-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="14bc1-104">Щоб розблокувати Windows 10 за допомогою відбитків пальців, потрібно налаштувати Windows Hello Fingerprint, додавши принаймні один палець (даючи Windows змогу навчитися розпізнавати).</span><span class="sxs-lookup"><span data-stu-id="14bc1-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="14bc1-105">Виберіть елементи **Настройки > Облікові > параметри входу** (або клацніть [тут).](ms-settings:signinoptions?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="14bc1-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="14bc1-106">З'являться доступні параметри входу.</span><span class="sxs-lookup"><span data-stu-id="14bc1-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="14bc1-107">Наприклад:</span><span class="sxs-lookup"><span data-stu-id="14bc1-107">For example:</span></span>

    ![Параметри входу.](media/sign-in-options.png)

2. <span data-ttu-id="14bc1-109">Виберіть **Відбиток пальця Windows Hello**, а потім натисніть **кнопку Настроїти**.</span><span class="sxs-lookup"><span data-stu-id="14bc1-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="14bc1-110">У вікні налаштування Windows Hello натисніть кнопку **Початок роботи.**</span><span class="sxs-lookup"><span data-stu-id="14bc1-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="14bc1-111">Датчик відбитків пальців активується, і вам буде запропоновано розмістити палець на датчик.</span><span class="sxs-lookup"><span data-stu-id="14bc1-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Датчик відбитків пальців.](media/fingerprint-sensor.png)

3. <span data-ttu-id="14bc1-113">Дотримуйтеся вказівок із проханням неодноразово просканувати палець.</span><span class="sxs-lookup"><span data-stu-id="14bc1-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="14bc1-114">Коли все буде готово, ви зможете додати інші пальці, які ви можете використовувати для входу.</span><span class="sxs-lookup"><span data-stu-id="14bc1-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="14bc1-115">Під час наступного входу у Windows 10 у вас буде можливість використовувати відбиток пальця для цього.</span><span class="sxs-lookup"><span data-stu-id="14bc1-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="14bc1-116">**Windows Hello Fingerprint not available as a sign-in option**</span><span class="sxs-lookup"><span data-stu-id="14bc1-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="14bc1-117">Якщо у параметрах входу у Windows Hello немає параметра Відбиток відбитків пальців, це означає, що Windows не відомо про **будь-який** сканер відбитків пальців, підключених до КОМП'ютера, або що системна політика перешкоджає її використанню (якщо, наприклад, ПК керує на робочому місці).</span><span class="sxs-lookup"><span data-stu-id="14bc1-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="14bc1-118">Щоб усунути несправностей, виконайте</span><span class="sxs-lookup"><span data-stu-id="14bc1-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="14bc1-119">Натисніть кнопку **Пуск** на панелі завдань і знайдіть **диспетчер пристроїв.**</span><span class="sxs-lookup"><span data-stu-id="14bc1-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="14bc1-120">Клацніть або торкніться екрана, щоб **відкрити Диспетчер пристроїв**.</span><span class="sxs-lookup"><span data-stu-id="14bc1-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="14bc1-121">У диспетчері пристроїв розгорніть біометричні пристрої, клацнувши кутові шеврони.</span><span class="sxs-lookup"><span data-stu-id="14bc1-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Біометричні пристрої.](media/biometric-devices.png)

4. <span data-ttu-id="14bc1-123">Сканер відбитків пальців має бути зазначено як біометричний пристрій, наприклад сканер Synaptics WBDI.</span><span class="sxs-lookup"><span data-stu-id="14bc1-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Біометричні пристрої.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="14bc1-125">Якщо сканер відбитків пальців не відображається, а сканер інтегровано в ПК, перейдіть на веб-сайт виробника ПК.</span><span class="sxs-lookup"><span data-stu-id="14bc1-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="14bc1-126">У розділі технічної підтримки для моделі ПК знайдіть драйвер Windows 10, який можна інсталювати.</span><span class="sxs-lookup"><span data-stu-id="14bc1-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="14bc1-127">Якщо сканер відокремлено від КОМП'ютера (підключено через USB), перейдіть на веб-сайт виробника сканера, щоб знайти й інсталювати драйвер пристрою з Windows 10 для інстальованої моделі сканера.</span><span class="sxs-lookup"><span data-stu-id="14bc1-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
