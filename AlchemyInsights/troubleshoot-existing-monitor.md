---
title: Виправлення неполадок із наявним монітором
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690732"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="ea185-102">Виправлення неполадок із наявним монітором</span><span class="sxs-lookup"><span data-stu-id="ea185-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="ea185-103">Скористайтеся цими рішеннями, щоб усунути несправності монітора.</span><span class="sxs-lookup"><span data-stu-id="ea185-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="ea185-104">**Оновіть екран монітора:**</span><span class="sxs-lookup"><span data-stu-id="ea185-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="ea185-105">Натискайте такі клавіші одночасно: клавіша Windows + Ctrl + Shift + B. Це оновлюватиме зв'язок із графічним драйвером.</span><span class="sxs-lookup"><span data-stu-id="ea185-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="ea185-106">Ваші монітори миттєво блимають та повертаються через кілька секунд.</span><span class="sxs-lookup"><span data-stu-id="ea185-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="ea185-107">**Виправлення неполадок із устаткуванням монітора:**</span><span class="sxs-lookup"><span data-stu-id="ea185-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="ea185-108">Від'єднайте кабель для підключення ПК до монітора та підключіть його знову.</span><span class="sxs-lookup"><span data-stu-id="ea185-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="ea185-109">Відключіть всі несуттєві пристрої на ПК (наприклад, адаптери або доки).</span><span class="sxs-lookup"><span data-stu-id="ea185-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="ea185-110">**Якщо ви нещодавно інсталювали оновлення на ПК, ви можете повернути драйвер дисплея.**</span><span class="sxs-lookup"><span data-stu-id="ea185-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="ea185-111">Натисніть кнопку **Пуск**, введіть **Диспетчер пристроїв**, а потім виберіть **Диспетчер пристроїв** із результатів.</span><span class="sxs-lookup"><span data-stu-id="ea185-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ea185-112">Розгорніть розділ **відображення адаптерів** , клацніть правою кнопкою миші адаптер, а потім виберіть **Властивості**.</span><span class="sxs-lookup"><span data-stu-id="ea185-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="ea185-113">Перейдіть на вкладку **драйвер** і натисніть кнопку **відкотити драйвер**.</span><span class="sxs-lookup"><span data-stu-id="ea185-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="ea185-114">Примітка. Якщо ця функція недоступна або недоступна, виберіть пункт **ні** з наведених нижче варіантів, щоб переходити до наступного кроку.</span><span class="sxs-lookup"><span data-stu-id="ea185-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="ea185-115">Щоб ці зміни набрали сили, може знадобитися перезавантажити комп'ютер.</span><span class="sxs-lookup"><span data-stu-id="ea185-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="ea185-116">**Видаліть і повторно інсталюйте драйвер дисплея.**</span><span class="sxs-lookup"><span data-stu-id="ea185-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="ea185-117">Натисніть кнопку **Пуск**, введіть **Диспетчер пристроїв**, а потім виберіть **Диспетчер пристроїв** із результатів.</span><span class="sxs-lookup"><span data-stu-id="ea185-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="ea185-118">Розгорніть розділ " **відображення адаптерів** ", клацніть правою кнопкою миші адаптер дисплея, а потім виберіть **Видалити пристрій**.</span><span class="sxs-lookup"><span data-stu-id="ea185-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="ea185-119">Установіть прапорець поруч із пунктом **видалити програмне забезпечення драйвера для цього пристрою** та натисніть кнопку **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="ea185-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="ea185-120">Примітка: можливо, вам буде запропоновано перезавантажити комп'ютер на цьому етапі.</span><span class="sxs-lookup"><span data-stu-id="ea185-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="ea185-121">Перед перезавантаженням переконайтеся, що ви записуємо решту інструкцій.</span><span class="sxs-lookup"><span data-stu-id="ea185-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="ea185-122">Відкрийте диспетчер пристроїв ще раз.</span><span class="sxs-lookup"><span data-stu-id="ea185-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="ea185-123">Розгорніть розділ **відображення адаптерів** , клацніть правою кнопкою миші на екрані адаптера та виберіть **оновити драйвер**.</span><span class="sxs-lookup"><span data-stu-id="ea185-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="ea185-124">Натисніть кнопку **Пошук автоматично для драйвера оновлення програмного забезпечення** та дотримуйтесь інструкцій з інсталяції.</span><span class="sxs-lookup"><span data-stu-id="ea185-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>