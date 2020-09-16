---
title: Виправлення неполадок із Bluetooth у Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730180"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="288fc-102">Виправлення неполадок із Bluetooth у Windows 10</span><span class="sxs-lookup"><span data-stu-id="288fc-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="288fc-103">Якщо піктограма Bluetooth відсутня або не можна ввімкнути або вимкнути Bluetooth, можливо, знадобиться запустити засіб усунення неполадок Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="288fc-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="288fc-104">[Відкрийте параметри виправлення неполадок](ms-settings:troubleshoot), виберіть елемент **Bluetooth** у розділі **знайти та виправити інші неполадки**, виберіть команду **запустити засіб усунення неполадок**.</span><span class="sxs-lookup"><span data-stu-id="288fc-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="288fc-105">Якщо піктограма Bluetooth не відображається, але Bluetooth відображається в диспетчері пристроїв:</span><span class="sxs-lookup"><span data-stu-id="288fc-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="288fc-106">У диспетчері пристроїв натисніть кнопку **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="288fc-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="288fc-107">Натисніть і утримуйте (або клацніть правою кнопкою миші) ім'я адаптера Bluetooth і натисніть кнопку **Видалити пристрій**.</span><span class="sxs-lookup"><span data-stu-id="288fc-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="288fc-108">Завершіть роботу пристрою з Windows, Зачекайте кілька секунд, а потім знову ввімкніть.</span><span class="sxs-lookup"><span data-stu-id="288fc-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="288fc-109">Операційна система Windows спробує повторно інсталювати драйвер.</span><span class="sxs-lookup"><span data-stu-id="288fc-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="288fc-110">Якщо ви нещодавно інсталювали оновлення Windows 10 або оновили систему до Windows 10, можливо, потрібно перевірити наявність оновлень драйверів:</span><span class="sxs-lookup"><span data-stu-id="288fc-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="288fc-111">У диспетчері пристроїв натисніть кнопку **Bluetooth**, а потім виберіть ім'я адаптера Bluetooth (що може містити слово "радіо").</span><span class="sxs-lookup"><span data-stu-id="288fc-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="288fc-112">Натисніть і утримуйте (або клацніть правою кнопкою миші) адаптер Bluetooth, а потім виберіть пункт **оновити**  >  **пошук драйверів автоматично для оновленого програмного забезпечення драйвера**.</span><span class="sxs-lookup"><span data-stu-id="288fc-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="288fc-113">Виконайте наведені нижче дії, а потім натисніть кнопку **закрити**.</span><span class="sxs-lookup"><span data-stu-id="288fc-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="288fc-114">Якщо Windows не вдалося знайти новий драйвер Bluetooth, перейдіть на веб-сайт виробника ПК та завантажте найновіший драйвер Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="288fc-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="288fc-115">Завантаживши його, натисніть кнопку **оновити драйвер**, перейдіть на  >  **комп'ютер для програмного забезпечення драйверів**, щоб  >  **знайти** розташування, у якому файли драйвера зберігаються > **OK**  >  **Далі**, і дотримуйтеся вказівок, щоб інсталювати.</span><span class="sxs-lookup"><span data-stu-id="288fc-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="288fc-116">Після інсталяції оновленого драйвера перезавантажте комп'ютер, а потім перевірте, чи це усуває проблему з підключенням.</span><span class="sxs-lookup"><span data-stu-id="288fc-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="288fc-117">Докладні відомості про виправлення неполадок із Bluetooth наведено в статті повна стаття, [Виправлення неполадок із Bluetooth у Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="288fc-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
