---
title: Виправлення неполадок Bluetooth у Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268714"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="b65b8-102">Виправлення неполадок Bluetooth у Windows 10</span><span class="sxs-lookup"><span data-stu-id="b65b8-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="b65b8-103">Якщо піктограма Bluetooth відсутня, або Bluetooth не можна ввімкнути або вимкнути, можливо, потрібно запустити засіб усунення неполадок Bluetooth.</span><span class="sxs-lookup"><span data-stu-id="b65b8-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="b65b8-104">[Відкрийте параметри виправлення неполадок](ms-settings:troubleshoot), клацніть **Bluetooth** у розділі **знайти та виправити інші неполадки**, виберіть пункт **запустити засіб усунення неполадок**.</span><span class="sxs-lookup"><span data-stu-id="b65b8-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="b65b8-105">Якщо піктограма Bluetooth не відображається, але Bluetooth відображається в диспетчері пристроїв:</span><span class="sxs-lookup"><span data-stu-id="b65b8-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="b65b8-106">У диспетчері пристроїв натисніть кнопку **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="b65b8-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="b65b8-107">Натисніть і утримуйте (або клацніть правою кнопкою миші) ім'я адаптера Bluetooth і натисніть кнопку **Видалити пристрій**.</span><span class="sxs-lookup"><span data-stu-id="b65b8-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="b65b8-108">Завершіть роботу пристрою Windows, Зачекайте кілька секунд, а потім знову ввімкніть його.</span><span class="sxs-lookup"><span data-stu-id="b65b8-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="b65b8-109">Windows спробує переінсталювати драйвер.</span><span class="sxs-lookup"><span data-stu-id="b65b8-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="b65b8-110">Якщо ви нещодавно інсталювали оновлення Windows 10 або оновили систему до Windows 10, можливо, потрібно перевірити наявність оновлень драйверів.</span><span class="sxs-lookup"><span data-stu-id="b65b8-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="b65b8-111">У диспетчері пристроїв клацніть **Bluetooth**, а потім клацніть ім'я адаптера Bluetooth (який може містити слово "радіо").</span><span class="sxs-lookup"><span data-stu-id="b65b8-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="b65b8-112">Натисніть і утримуйте (або клацніть правою кнопкою миші) адаптер Bluetooth і виберіть пункт **оновити драйвер** > **пошуку автоматично для оновлених драйверів**.</span><span class="sxs-lookup"><span data-stu-id="b65b8-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="b65b8-113">Виконайте дії, а потім натисніть кнопку **закрити**.</span><span class="sxs-lookup"><span data-stu-id="b65b8-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="b65b8-114">Якщо Windows не вдається знайти новий драйвер Bluetooth, відвідайте веб-сайт виробника комп'ютера та завантажте найновіший драйвер Bluetooth звідти.</span><span class="sxs-lookup"><span data-stu-id="b65b8-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="b65b8-115">Після завантаження натисніть кнопку " **оновити драйвер** > "**перегляньте мій комп'ютер для програмного забезпечення** > драйвера**знайдіть** розташування, де зберігаються файли драйверів > **ОК** > **Далі**та дотримуйтеся вказівок для інсталяції.</span><span class="sxs-lookup"><span data-stu-id="b65b8-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="b65b8-116">Після інсталяції оновленого драйвера перезавантажте комп'ютер і перевірте, чи вирішено проблему з підключенням.</span><span class="sxs-lookup"><span data-stu-id="b65b8-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="b65b8-117">Щоб отримати додаткові відомості про виправлення неполадок Bluetooth, перегляньте статтю повністю, [виправте неполадки Bluetooth у Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="b65b8-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
