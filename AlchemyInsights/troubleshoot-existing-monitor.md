---
title: Виправлення неполадок із наявним монітором
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824600"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="84ba2-102">Виправлення неполадок із наявним монітором</span><span class="sxs-lookup"><span data-stu-id="84ba2-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="84ba2-103">Скористайтеся цими рішеннями, щоб усунути несправностей із монітором.</span><span class="sxs-lookup"><span data-stu-id="84ba2-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="84ba2-104">**Оновлення дисплея монітора.**</span><span class="sxs-lookup"><span data-stu-id="84ba2-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="84ba2-105">Одночасно натисніть такі клавіші: Клавіша Windows + Ctrl + Shift + B. Це оновить зв'язок із графічним драйвером.</span><span class="sxs-lookup"><span data-stu-id="84ba2-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="84ba2-106">Монітори миготять і повертаються через кілька секунд.</span><span class="sxs-lookup"><span data-stu-id="84ba2-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="84ba2-107">**Усунення несправностей із обладнанням монітора.**</span><span class="sxs-lookup"><span data-stu-id="84ba2-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="84ba2-108">Від'єднайте кабель, підключивши комп'ютер до монітора, і знову під'єднайте його.</span><span class="sxs-lookup"><span data-stu-id="84ba2-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="84ba2-109">Відключіть від ПК всі несуть важливі пристрої (наприклад, адаптери або док-станцію).</span><span class="sxs-lookup"><span data-stu-id="84ba2-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="84ba2-110">**Якщо ви нещодавно інсталювали оновлення на ПК, можна відкотити драйвер дисплея:**</span><span class="sxs-lookup"><span data-stu-id="84ba2-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="84ba2-111">Натисніть **кнопку Пуск**, **введіть диспетчер** пристроїв і виберіть **у** списку результатів пункт Диспетчер пристроїв.</span><span class="sxs-lookup"><span data-stu-id="84ba2-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="84ba2-112">**Розгорніть розділ Відеоадаптери,** клацніть правою кнопкою миші відеоадаптер і виберіть **пункт Властивості**.</span><span class="sxs-lookup"><span data-stu-id="84ba2-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="84ba2-113">Перейдіть на вкладку Драйвер **і** виберіть **Відкотити драйвер.**</span><span class="sxs-lookup"><span data-stu-id="84ba2-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="84ba2-114">Примітка. Якщо цей пункт недоступний або він недоступний, виберіть Ні в меню нижче, щоб перейти до наступного кроку. </span><span class="sxs-lookup"><span data-stu-id="84ba2-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="84ba2-115">Можливо, перш ніж ці зміни наберуть сили, знадобиться перезавантажити комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="84ba2-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="84ba2-116">**Видаліть і повторно інсталюйте драйвер дисплея.**</span><span class="sxs-lookup"><span data-stu-id="84ba2-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="84ba2-117">Натисніть **кнопку Пуск**, **введіть диспетчер** пристроїв і виберіть **у** списку результатів пункт Диспетчер пристроїв.</span><span class="sxs-lookup"><span data-stu-id="84ba2-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="84ba2-118">**Розгорніть розділ** Відеоадаптери, клацніть відеоадаптер правою кнопкою миші й виберіть **Видалити пристрій.**</span><span class="sxs-lookup"><span data-stu-id="84ba2-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="84ba2-119">Установіть прапорець поруч із **пунктом Видалити драйвер для цього пристрою та** натисніть кнопку **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="84ba2-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="84ba2-120">Примітка. На цьому етапі може з'явитися запит на перезавантаження комп'ютера.</span><span class="sxs-lookup"><span data-stu-id="84ba2-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="84ba2-121">Обов'язково запишіть решту інструкцій, перш ніж перезапустити програму.</span><span class="sxs-lookup"><span data-stu-id="84ba2-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="84ba2-122">Знову відкрийте диспетчер пристроїв.</span><span class="sxs-lookup"><span data-stu-id="84ba2-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="84ba2-123">**Розгорніть розділ** Відеоадаптери, клацніть правою кнопкою миші відеоадаптер і виберіть **команду Оновити драйвер.**</span><span class="sxs-lookup"><span data-stu-id="84ba2-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="84ba2-124">Виберіть **автоматично шукати драйвер оновлення та** дотримуйтеся вказівок з інсталяції.</span><span class="sxs-lookup"><span data-stu-id="84ba2-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>