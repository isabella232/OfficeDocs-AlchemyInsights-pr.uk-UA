---
title: Вирішення проблем із Bluetooth у Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812953"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="d41be-102">Вирішення проблем із Bluetooth у Windows 10</span><span class="sxs-lookup"><span data-stu-id="d41be-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="d41be-103">Якщо піктограма Bluetooth відсутня або bluetooth не вдається ввімкнути або вимкнути, можливо, потрібно запустити засіб усунення неполадок із Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="d41be-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="d41be-104">[Відкрийте настройки Виправлення неполадок](ms-settings:troubleshoot), у розділі Пошук **і** вирішення інших **проблем** клацніть елемент Запустити засіб **усунення неполадок.**</span><span class="sxs-lookup"><span data-stu-id="d41be-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="d41be-105">Якщо піктограма Bluetooth не відображається, але в диспетчері пристроїв відображається така піктограма Bluetooth:</span><span class="sxs-lookup"><span data-stu-id="d41be-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="d41be-106">У диспетчері пристроїв натисніть **кнопку Bluetooth.**</span><span class="sxs-lookup"><span data-stu-id="d41be-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="d41be-107">Натисніть і утримуйте (або клацніть правою кнопкою миші) ім'я адаптера Bluetooth і виберіть **видалити пристрій**.</span><span class="sxs-lookup"><span data-stu-id="d41be-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="d41be-108">Вимкніть пристрій Windows, зачекайте кілька секунд, а потім увімкніть його знову.</span><span class="sxs-lookup"><span data-stu-id="d41be-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="d41be-109">Windows спробує повторно інсталювати драйвер.</span><span class="sxs-lookup"><span data-stu-id="d41be-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="d41be-110">Якщо ви нещодавно інсталюли оновлення Windows 10 або оновили ОС до Windows 10, перевірте наявність оновлень драйверів.</span><span class="sxs-lookup"><span data-stu-id="d41be-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="d41be-111">У диспетчері пристроїв клацніть **Bluetooth**, а потім клацніть ім'я адаптера Bluetooth (яке може містити слово "radio").</span><span class="sxs-lookup"><span data-stu-id="d41be-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="d41be-112">Натисніть і утримуйте (або клацніть правою кнопкою миші) адаптер Bluetooth, а потім виберіть Автоматично оновлювати пошук драйверів для  >  **оновленого драйвера**.</span><span class="sxs-lookup"><span data-stu-id="d41be-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="d41be-113">Дотримуйтеся вказівок, а потім натисніть кнопку **Закрити.**</span><span class="sxs-lookup"><span data-stu-id="d41be-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="d41be-114">Якщо Windows не вдається знайти новий драйвер Bluetooth, відвідайте веб-сайт виробника ПК та завантажте звідти останню версію драйвера Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="d41be-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="d41be-115">Завантаживши драйвер >, натисніть кнопку Оновити драйвер. Знайдіть розташування, у якому зберігаються файли драйверів, і виконайте вказівки з  >    >     >  інсталяції.</span><span class="sxs-lookup"><span data-stu-id="d41be-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="d41be-116">Після інсталяції оновленого драйвера перезавантажте комп'ютер і перевірте, чи вирішено проблему з підключенням.</span><span class="sxs-lookup"><span data-stu-id="d41be-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="d41be-117">Докладні відомості про виправлення неполадок із Bluetooth див. в повній статті Вирішення проблем [із Bluetooth у Windows 10.](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)</span><span class="sxs-lookup"><span data-stu-id="d41be-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
