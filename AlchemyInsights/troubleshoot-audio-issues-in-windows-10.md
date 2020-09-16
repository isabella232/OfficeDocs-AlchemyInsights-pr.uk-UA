---
title: Виправлення неполадок із звуком у Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750364"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="e11e4-102">Виправлення неполадок із звуком у Windows 10</span><span class="sxs-lookup"><span data-stu-id="e11e4-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="e11e4-103">**Запуск засобу усунення неполадок із відтворенням звуку**</span><span class="sxs-lookup"><span data-stu-id="e11e4-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="e11e4-104">Відкрийте [Параметри виправлення неполадок](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="e11e4-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="e11e4-105">Натисніть кнопку **відтворення звуку**  >  **, щоб запустити засіб усунення неполадок**.</span><span class="sxs-lookup"><span data-stu-id="e11e4-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="e11e4-106">**Установлення стандартного пристрою**</span><span class="sxs-lookup"><span data-stu-id="e11e4-106">**Set the default device**</span></span>

<span data-ttu-id="e11e4-107">Якщо ви підключаєтеся до аудіопристрою за допомогою USB або HDMI, можливо, знадобиться встановити цей пристрій за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="e11e4-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="e11e4-108">Відкрийте **початковий**  >  **звук**, а потім у списку результатів виберіть **звук** або **змінити системні звуки** .</span><span class="sxs-lookup"><span data-stu-id="e11e4-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="e11e4-109">На вкладці **відтворити** виберіть пристрій, а потім натисніть кнопку **Установити за замовчуванням**, а потім – **OK**.</span><span class="sxs-lookup"><span data-stu-id="e11e4-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="e11e4-110">**Перевірка кабелів, об'ємних, динаміків і навушників**</span><span class="sxs-lookup"><span data-stu-id="e11e4-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="e11e4-111">Перевірте підключення динаміків і навушників для сипучих кабелів і переконайтеся, що вони підключені до правильного розніму.</span><span class="sxs-lookup"><span data-stu-id="e11e4-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="e11e4-112">Перевірте рівень живлення та гучності та спробуйте ввімкнути всі елементи керування томом.</span><span class="sxs-lookup"><span data-stu-id="e11e4-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="e11e4-113">Деякі динаміки та програми мають власні елементи керування томом; Можливо, вам доведеться перевіряти їх усі, щоб переконатися, що вони знаходяться на рівні потрібних рівнів.</span><span class="sxs-lookup"><span data-stu-id="e11e4-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="e11e4-114">Випробуйте підключення за допомогою іншого USB-порту.</span><span class="sxs-lookup"><span data-stu-id="e11e4-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="e11e4-115">**Зверніть увагу**: Пам'ятайте, що динаміки можуть не працювати, коли навушники підключено.</span><span class="sxs-lookup"><span data-stu-id="e11e4-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="e11e4-116">**Перевірка диспетчера пристроїв**</span><span class="sxs-lookup"><span data-stu-id="e11e4-116">**Check Device Manager**</span></span>

<span data-ttu-id="e11e4-117">Щоб забезпечити оновлення драйверів, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="e11e4-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="e11e4-118">Натисніть кнопку **Пуск**, введіть **Диспетчер пристроїв**, а потім виберіть **Диспетчер пристроїв** зі списку результатів.</span><span class="sxs-lookup"><span data-stu-id="e11e4-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="e11e4-119">У розділі **аудіо-, відео-та ігрові контролери**виберіть звукову плату, відкрийте його, перейдіть на вкладку **драйвер** і натисніть кнопку **оновити драйвер**.</span><span class="sxs-lookup"><span data-stu-id="e11e4-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="e11e4-120">**Примітка**. Якщо Windows не знаходить нового драйвера, знайдіть його на веб-сайті виробника пристрою та дотримуйтеся вказівок, наведених нижче.</span><span class="sxs-lookup"><span data-stu-id="e11e4-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="e11e4-121">**Повторна інсталяція драйвера**</span><span class="sxs-lookup"><span data-stu-id="e11e4-121">**Reinstall the driver**</span></span>

<span data-ttu-id="e11e4-122">Якщо не вдається оновити за допомогою диспетчера пристроїв або знайти новий драйвер на веб-сайті виробника, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="e11e4-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="e11e4-123">У диспетчері пристроїв клацніть правою кнопкою миші (або натисніть і утримуйте) драйвер звуку та натисніть кнопку **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="e11e4-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="e11e4-124">Перезавантажте пристрій і Windows спробує повторно інсталювати драйвер.</span><span class="sxs-lookup"><span data-stu-id="e11e4-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="e11e4-125">Якщо повторна інсталяція драйвера не працює, скористайтеся загальним драйвером звуку, який постачається з Windows.</span><span class="sxs-lookup"><span data-stu-id="e11e4-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="e11e4-126">У диспетчері пристроїв клацніть правою кнопкою миші (або натисніть і утримуйте) драйвер драйвера > **оновлення драйвера на**  >  комп'ютері, на якому інстальовано програмне**забезпечення для драйверів**,  >  **дозвольте мені вибрати зі списку драйверів пристроїв на моєму комп'ютері**, виберіть елемент **висока звукова пристрій визначення**, натисніть кнопку **Далі**, а потім дотримуйтеся вказівок, щоб інсталювати її.</span><span class="sxs-lookup"><span data-stu-id="e11e4-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
