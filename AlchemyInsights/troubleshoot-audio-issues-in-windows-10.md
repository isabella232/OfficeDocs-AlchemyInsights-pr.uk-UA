---
title: Усунення несправностей зі звуком у Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833312"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="c28e1-102">Виправлення неполадок зі звуком у Windows 10</span><span class="sxs-lookup"><span data-stu-id="c28e1-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="c28e1-103">**Запуск засобу усунення неполадок звуку**</span><span class="sxs-lookup"><span data-stu-id="c28e1-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="c28e1-104">Відкрийте настройки [Виправлення неполадок.](ms-settings:troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="c28e1-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="c28e1-105">Виберіть **пункт Відтворення**  >  **звуку Запуск засобу усунення неполадок.**</span><span class="sxs-lookup"><span data-stu-id="c28e1-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="c28e1-106">**Установлення пристрою за замовчуванням**</span><span class="sxs-lookup"><span data-stu-id="c28e1-106">**Set the default device**</span></span>

<span data-ttu-id="c28e1-107">Якщо ви підключається до аудіопристрою за допомогою USB- або HDMI-кабелю, можливо, знадобиться зробити цей пристрій пристроєм за замовчуванням:</span><span class="sxs-lookup"><span data-stu-id="c28e1-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="c28e1-108">Відкрийте **меню Пуск** звуку , а потім виберіть зі списку результатів пункт Звук  >  або Змінення системних звуків.  </span><span class="sxs-lookup"><span data-stu-id="c28e1-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="c28e1-109">На **вкладці Відтворення виберіть** пристрій, клацніть Установити за **замовчуванням**, а потім натисніть кнопку **OK**.</span><span class="sxs-lookup"><span data-stu-id="c28e1-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="c28e1-110">**Перевірка кабелів, гучності, динаміків і навушників**</span><span class="sxs-lookup"><span data-stu-id="c28e1-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="c28e1-111">Перевірте підключення динаміка й навушників і переконайтеся, що кабелі відібрано, і переконайтеся, що їх підключено до відповідного гнізда.</span><span class="sxs-lookup"><span data-stu-id="c28e1-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="c28e1-112">Перевірте рівень живлення та гучності та спробуйте повернути всі регулятори гучності вгору.</span><span class="sxs-lookup"><span data-stu-id="c28e1-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="c28e1-113">Деякі динаміки та програми мають власні регулятори гучності; можливо, доведеться перевірити їх усі, щоб переконатися, що вони на правильних рівнях.</span><span class="sxs-lookup"><span data-stu-id="c28e1-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="c28e1-114">Спробуйте підключитися за допомогою іншого USB-порту.</span><span class="sxs-lookup"><span data-stu-id="c28e1-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="c28e1-115">**Примітка.** Пам'ятайте, що динаміки можуть не працювати, коли навушники підключено.</span><span class="sxs-lookup"><span data-stu-id="c28e1-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="c28e1-116">**Перевірка диспетчера пристроїв**</span><span class="sxs-lookup"><span data-stu-id="c28e1-116">**Check Device Manager**</span></span>

<span data-ttu-id="c28e1-117">Щоб переконатися в оновленні драйверів:</span><span class="sxs-lookup"><span data-stu-id="c28e1-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="c28e1-118">Натисніть **кнопку** Пуск , **введіть** Диспетчер пристроїв , а **потім** виберіть пункт Диспетчер пристроїв у списку результатів пошуку.</span><span class="sxs-lookup"><span data-stu-id="c28e1-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="c28e1-119">У **розділі Контролери звуку, відео та ігор** виберіть свою  звукову плату, відкрийте її, відкрийте вкладку Драйвер і натисніть кнопку **Оновити драйвер**.</span><span class="sxs-lookup"><span data-stu-id="c28e1-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="c28e1-120">**Примітка.** Якщо Windows не вдається знайти новий драйвер, знайдіть його на веб-сайті виробника пристрою та дотримуйтеся вказівок.</span><span class="sxs-lookup"><span data-stu-id="c28e1-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="c28e1-121">**Повторно інсталюйте драйвер**</span><span class="sxs-lookup"><span data-stu-id="c28e1-121">**Reinstall the driver**</span></span>

<span data-ttu-id="c28e1-122">Якщо не вдається оновити пакет за допомогою диспетчера пристроїв або знайти новий драйвер на веб-сайті виробника, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="c28e1-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="c28e1-123">У диспетчері пристроїв клацніть драйвер правою кнопкою миші (або натисніть і утримуйте) і виберіть команду **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="c28e1-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="c28e1-124">Перезавантажте пристрій, і Windows спробує повторно інсталювати драйвер.</span><span class="sxs-lookup"><span data-stu-id="c28e1-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="c28e1-125">Якщо повторна інсталяція драйвера не працює, спробуйте скористатися універсальним аудіо драйвером, який постачається разом із Windows.</span><span class="sxs-lookup"><span data-stu-id="c28e1-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="c28e1-126">У диспетчері пристроїв клацніть драйвер правою кнопкою миші (або натисніть і утримуйте) драйвер > Оновити драйвер Перегляньте програмне забезпечення драйвера на моєму комп'ютері Виберіть драйвер зі списку драйверів пристрою на комп'ютері , виберіть Аудіопристрій високої чіткості , натисніть кнопку Далі та дотримуйтеся вказівок, щоб  >    >  інсталювати його.  </span><span class="sxs-lookup"><span data-stu-id="c28e1-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
