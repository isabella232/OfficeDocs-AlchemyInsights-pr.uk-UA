---
title: Піктограма живлення або акумулятора не відображається у Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790569"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="ee5c4-102">Піктограма живлення або акумулятора не відображається у Windows 10</span><span class="sxs-lookup"><span data-stu-id="ee5c4-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="ee5c4-103">Якщо у вашому пристрої з Windows 10 є акумулятор (наприклад, ноутбук або планшет чи ПК, підключений через USB до ДБЖ), зазвичай на панелі завдань поруч із годинником відображається піктограма живлення/акумулятора, наприклад:</span><span class="sxs-lookup"><span data-stu-id="ee5c4-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Піктограма акумулятора](media/battery-icon.png)

<span data-ttu-id="ee5c4-105">Якщо піктограму не видно, можливо, її приховано.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="ee5c4-106">Перейдіть у меню **[Параметри > Персоналізація > Панель завдань](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="ee5c4-107">В області сповіщень натисніть **Вибрати, які піктограми показувати на панелі завдань**.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="ee5c4-108">У списку знайдіть елемент **Живлення** й установіть його перемикач у положення **Увімк.**.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Показ піктограми живлення на панелі завдань](media/power-icon-on.png)

<span data-ttu-id="ee5c4-110">**Виправлення неполадок**</span><span class="sxs-lookup"><span data-stu-id="ee5c4-110">**Troubleshooting**</span></span>

<span data-ttu-id="ee5c4-111">Якщо ви виконали вказані вище інструкції, але перемикач **Живлення** затінено або його не видно, у полі пошуку на панелі завдань введіть **диспетчер пристроїв** і виберіть **Диспетчер пристроїв** у списку результатів.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="ee5c4-112">У розділі **Акумулятори** натисніть правою кнопкою миші акумулятор свого пристрою та виберіть **Вимкнути**, а потім – **Так**.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="ee5c4-113">Зачекайте кілька секунд, а потім натисніть правою кнопкою миші акумулятор і виберіть **Увімкнути**.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="ee5c4-114">Перезавантажте пристрій.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-114">Then restart your device.</span></span>

<span data-ttu-id="ee5c4-115">Якщо ви виконали вказані вище інструкції, але піктограма акумулятора не з’явилася на панелі завдань, у полі пошуку на панелі завдань введіть **диспетчер завдань** і натисніть **Диспетчер завдань** у списку результатів.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="ee5c4-116">На вкладці **Процеси** в розділі **Назва** натисніть правою кнопкою миші **Провідник** і виберіть **Перезавантажити**.</span><span class="sxs-lookup"><span data-stu-id="ee5c4-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
