---
title: Виправлення неполадок із аудіо у Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 46b23f97c2e682258224dc95e7a76b1201991828
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/19/2019
ms.locfileid: "40796459"
---
# <a name="troubleshooting-audio-problems-in-windows-10"></a><span data-ttu-id="1a7ce-102">Виправлення неполадок із аудіопроблемами у Windows 10</span><span class="sxs-lookup"><span data-stu-id="1a7ce-102">Troubleshooting audio problems in Windows 10</span></span>

<span data-ttu-id="1a7ce-103">**Запуск засобу усунення неполадок звуку**</span><span class="sxs-lookup"><span data-stu-id="1a7ce-103">**Run the audio troubleshooter**</span></span>

<span data-ttu-id="1a7ce-104">Засіб усунення неполадок звуку може автоматично виправити неполадки аудіосупроводу:</span><span class="sxs-lookup"><span data-stu-id="1a7ce-104">The audio troubleshooter might be able to fix the audio problems automatically:</span></span> 

1. <span data-ttu-id="1a7ce-105">Натисніть кнопку **Пуск**, введіть **Виправлення неполадок**, а потім виберіть **Виправлення неполадок** зі списку результатів.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-105">Select **Start**, type **troubleshoot**, and then select **Troubleshoot** from the list of results.</span></span> 
2. <span data-ttu-id="1a7ce-106">Виберіть **відтворення аудіо** > **запустити засіб усунення неполадок**.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-106">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="1a7ce-107">**Перевірка кабелів, гучності, динаміків і навушників**</span><span class="sxs-lookup"><span data-stu-id="1a7ce-107">**Check cables, volume, speakers, and headphones**</span></span>

- <span data-ttu-id="1a7ce-108">Перевірте підключення динаміків і навушників для вільних кабелів і переконайтеся, що вони підключені до правильного розніму.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-108">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>
- <span data-ttu-id="1a7ce-109">Перевірте свої рівні живлення та гучність і спробуйте вимкнути всі елементи керування гучністю.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-109">Check your power and volume levels, and try turning all the volume controls up.</span></span>
- <span data-ttu-id="1a7ce-110">Деякі динаміки та додатки мають власні елементи керування гучністю, і вам, можливо, доведеться перевірити їх усі, щоб переконатися, що вони знаходяться на потрібних рівнях.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-110">Some speakers and apps have their own volume controls, and you might have to check them all to make sure they're at the right levels.</span></span>
- <span data-ttu-id="1a7ce-111">Спробуйте підключитися за допомогою іншого USB-порту.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-111">Try connecting using a different USB port.</span></span>
- <span data-ttu-id="1a7ce-112">**Примітка:** Пам'ятайте, що динаміки можуть не працювати, коли навушники підключено.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-112">**Note:** Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="1a7ce-113">**Перевірка диспетчера пристроїв**</span><span class="sxs-lookup"><span data-stu-id="1a7ce-113">**Check Device Manager**</span></span>

<span data-ttu-id="1a7ce-114">Щоб переконатися, що драйвери Оновлено:</span><span class="sxs-lookup"><span data-stu-id="1a7ce-114">To make sure the drivers are up to date:</span></span>

- <span data-ttu-id="1a7ce-115">Натисніть кнопку **Пуск**, введіть **Диспетчер пристроїв**, а потім виберіть **Диспетчер пристроїв** у списку результатів.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-115">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="1a7ce-116">У розділі **аудіо, відео та ігрові контролери**виберіть звукову плату, відкрийте її, перейдіть на вкладку **драйвер** і виберіть пункт **оновити драйвер**.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-116">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span> 

<span data-ttu-id="1a7ce-117">**Примітка:** Якщо Windows не вдається знайти новий драйвер, знайдіть його на веб-сайті виробника пристрою та дотримуйтеся вказівок на екрані.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-117">**Note:** If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="1a7ce-118">**Повторна інсталяція драйвера**</span><span class="sxs-lookup"><span data-stu-id="1a7ce-118">**Reinstall the driver**</span></span>

<span data-ttu-id="1a7ce-119">Якщо не вдається оновити за допомогою диспетчера пристроїв або знайти новий драйвер на веб-сайті виробника, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="1a7ce-119">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span> 

1. <span data-ttu-id="1a7ce-120">У диспетчері пристроїв клацніть правою кнопкою миші (або натисніть і утримуйте) аудіодрайвер і виберіть **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-120">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="1a7ce-121">Перезавантажте пристрій і Windows спробує переінсталювати драйвер.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-121">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="1a7ce-122">Якщо повторна інсталяція драйвера не працює, спробуйте скористатися загальним аудіодрайвером, який постачається з Windows.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-122">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="1a7ce-123">У диспетчері пристроїв клацніть правою кнопкою миші (або натисніть і утримуйте) звуковий драйвер > **оновити драйвер програмне забезпечення** > **Огляд мій комп'ютер для драйвера програмне забезпечення** > **дозвольте мені вибрати зі списку драйверів пристроїв на моєму комп'ютері**, виберіть **висока роздільна здатність аудіопристрій**, виберіть **Далі**, і дотримуйтесь інструкцій, щоб встановити його.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-123">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>

<span data-ttu-id="1a7ce-124">**Установлення пристрою за промовчанням**</span><span class="sxs-lookup"><span data-stu-id="1a7ce-124">**Set the default device**</span></span>

<span data-ttu-id="1a7ce-125">Якщо ви підключаєте пристрій до аудіопристрою за допомогою USB або HDMI, можливо, потрібно встановити цей пристрій за промовчанням:</span><span class="sxs-lookup"><span data-stu-id="1a7ce-125">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span> 

1. <span data-ttu-id="1a7ce-126">Натисніть кнопку **Пуск**, введіть **звук**, а потім виберіть **звук** або **змінити системні звуки** зі списку результатів.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-126">Select **Start**, type **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2. <span data-ttu-id="1a7ce-127">На вкладці **відтворення** виберіть пристрій, виберіть пункт **Установити за промовчанням**, а потім натисніть **кнопку OK**.</span><span class="sxs-lookup"><span data-stu-id="1a7ce-127">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

