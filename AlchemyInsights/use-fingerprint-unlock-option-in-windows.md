---
title: Використання параметра "розблокувати відбитки пальців" у Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795265"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="6040a-102">Використання параметра "розблокувати відбитки пальців" у Windows 10</span><span class="sxs-lookup"><span data-stu-id="6040a-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="6040a-103">**Увімкнення відбитків пальців Windows**</span><span class="sxs-lookup"><span data-stu-id="6040a-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="6040a-104">Щоб розблокувати Windows 10 за допомогою пальця, потрібно настроїти відбитки пальців з Windows, додавши (щоб ОС Windows дізнався, що ви дізналися) принаймні один палець.</span><span class="sxs-lookup"><span data-stu-id="6040a-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="6040a-105">Послідовно виберіть елементи **настройки > облікові записи > Параметри входу** (або клацніть [тут](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="6040a-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="6040a-106">Доступні варіанти входу буде наведено в списку.</span><span class="sxs-lookup"><span data-stu-id="6040a-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="6040a-107">Наприклад,</span><span class="sxs-lookup"><span data-stu-id="6040a-107">For example:</span></span>

    ![Варіанти входу.](media/sign-in-options.png)

2. <span data-ttu-id="6040a-109">Клацніть або торкніться елемента **Windows Hello відбитків пальців**, а потім натисніть кнопку **налаштувати**.</span><span class="sxs-lookup"><span data-stu-id="6040a-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="6040a-110">У вікні Настроювання Windows Здравствуйте натисніть кнопку початок **роботи**.</span><span class="sxs-lookup"><span data-stu-id="6040a-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="6040a-111">Сканер відбитків пальців буде активовано, і вам буде запропоновано розташувати пальцем на сенсорному екрані.</span><span class="sxs-lookup"><span data-stu-id="6040a-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Датчик пальця.](media/fingerprint-sensor.png)

3. <span data-ttu-id="6040a-113">Дотримуйтеся вказівок, у яких буде запропоновано повторно відсканувати пальцем.</span><span class="sxs-lookup"><span data-stu-id="6040a-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="6040a-114">Коли все буде Готово, ви матимете можливість додавати інші пальці, які можуть знадобитися для входу.</span><span class="sxs-lookup"><span data-stu-id="6040a-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="6040a-115">Під час наступного входу у Windows 10 у вас буде можливість використовувати відбитки пальців.</span><span class="sxs-lookup"><span data-stu-id="6040a-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="6040a-116">**У Windows Hello відбитків пальців немає в якості параметра входу**</span><span class="sxs-lookup"><span data-stu-id="6040a-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="6040a-117">Якщо у **вікні параметрів входу**не відображається функція "відбитки пальців Windows", це означає, що Windows не знає, чи сканер відбитків пальців, ПІДКЛЮЧЕНИЙ до ПК, або про те, що системна політика перешкоджає її використанню (якщо, наприклад, ваш ПК керує вашим робочим місцем).</span><span class="sxs-lookup"><span data-stu-id="6040a-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="6040a-118">Щоб виправити неполадки, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="6040a-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="6040a-119">Натисніть кнопку **Пуск** на панелі завдань і знайдіть **Диспетчер пристроїв**.</span><span class="sxs-lookup"><span data-stu-id="6040a-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="6040a-120">Щоб відкрити **Диспетчер пристроїв**, натисніть кнопку або торкніться його.</span><span class="sxs-lookup"><span data-stu-id="6040a-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="6040a-121">У диспетчері пристроїв розгорніть елемент Біометричні пристрої, клацнувши її Шеврон.</span><span class="sxs-lookup"><span data-stu-id="6040a-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Біометричні пристрої.](media/biometric-devices.png)

4. <span data-ttu-id="6040a-123">Сканер відбитків пальців має бути вказаний як Біометричні пристрої, наприклад сканер Synaptics WWDI:</span><span class="sxs-lookup"><span data-stu-id="6040a-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Біометричні пристрої.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="6040a-125">Якщо сканер відбитків пальців не відображається, а сканер інтегровано до ПК, перейдіть на веб-сайт виробника ПК.</span><span class="sxs-lookup"><span data-stu-id="6040a-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="6040a-126">У розділі технічної підтримки для моделі ПК знайдіть драйвер Windows 10 для сканера, який можна інсталювати.</span><span class="sxs-lookup"><span data-stu-id="6040a-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="6040a-127">Якщо сканер відділено від ПК (підключений через USB), перейдіть на веб-сайт виробника сканера, щоб знайти та інсталювати програмне забезпечення пристрою з Windows 10 із драйверами для сканера.</span><span class="sxs-lookup"><span data-stu-id="6040a-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
