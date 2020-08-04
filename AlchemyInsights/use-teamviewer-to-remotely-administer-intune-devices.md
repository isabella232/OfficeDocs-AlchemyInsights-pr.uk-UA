---
title: Використання TeamViewer для віддаленого адміністрування InTune пристроїв
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555754"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="cb187-102">Використання TeamViewer для віддаленого адміністрування InTune пристроїв</span><span class="sxs-lookup"><span data-stu-id="cb187-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="cb187-103">Пристрої, керовані InTune, можна адмініструватися віддалено за допомогою [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="cb187-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="cb187-104">Для адміністрування InTune за допомогою TeamViewer, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="cb187-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="cb187-105">Почніть з отримання облікових даних TeamViewer для налаштування з'єднувача TeamViewer на InTune.</span><span class="sxs-lookup"><span data-stu-id="cb187-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="cb187-106">Це дає змогу адміністратору вводити облікові дані в ІНТЕРФЕЙСІ-з'єднувача TeamViewer у розділі пристрої, операції з одним часом для встановлення зв'язку між InTune та службою TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="cb187-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="cb187-107">**Частина 1: запуск сеансу із віддаленим пристроєм**</span><span class="sxs-lookup"><span data-stu-id="cb187-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="cb187-108">У розділі **усі пристрої**виберіть пристрій, з якого потрібно почати віддалене сеанс.</span><span class="sxs-lookup"><span data-stu-id="cb187-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="cb187-109">Від **... Більше**, виберіть **нова сесія віддаленої допомоги**.</span><span class="sxs-lookup"><span data-stu-id="cb187-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="cb187-110">Виберіть **так** , щоб підтвердити, що потрібно встановити віддалений сеанс.</span><span class="sxs-lookup"><span data-stu-id="cb187-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="cb187-111">Після того, як запит "ініціювання нової віддаленої сесії" визнається службою TeamViewer, ви побачите можливість **запуску віддаленої допомоги** в деталях області огляду (або, основ) для пристрою.</span><span class="sxs-lookup"><span data-stu-id="cb187-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="cb187-112">Виберіть **Переглянути більше** , щоб розгорнути панель і показати стан віддаленої допомоги.</span><span class="sxs-lookup"><span data-stu-id="cb187-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="cb187-113">Виберіть **запустити віддалений сеанс** , щоб ініціювати сеанс на стороні адміністратора.</span><span class="sxs-lookup"><span data-stu-id="cb187-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="cb187-114">Виберіть завантажити двійковий файл TeamViewer (Windows) і виберіть **запустити**.</span><span class="sxs-lookup"><span data-stu-id="cb187-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="cb187-115">**Зверніть увагу** Ви можете ігнорувати будь-яку сторінку веб-браузера, відкриту до веб-сайту TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="cb187-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="cb187-116">Визначи запит на додаток TeamViewer для внесення змін до пристрою (лише для Windows).</span><span class="sxs-lookup"><span data-stu-id="cb187-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="cb187-117">Застосунок TeamViewer запускається та містить код сеансу для автентифікації підключення до віддаленого пристрою.</span><span class="sxs-lookup"><span data-stu-id="cb187-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="cb187-118">**Частина 2: на пристрої, орієнтовані на віддалений сеанс**</span><span class="sxs-lookup"><span data-stu-id="cb187-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="cb187-119">Відкрийте портал компанії InTune.</span><span class="sxs-lookup"><span data-stu-id="cb187-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="cb187-120">Знайдіть позначку сповіщення: "ваш адміністратор надсилає запит на керування цим пристроєм для сеансу віддаленої допомоги" і виберіть сповіщення.</span><span class="sxs-lookup"><span data-stu-id="cb187-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="cb187-121">Виберіть завантажити програму TeamViewer або визнаєте завантаження програми TeamViewer з магазину додатків і виберіть **запустити**.</span><span class="sxs-lookup"><span data-stu-id="cb187-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="cb187-122">**Зверніть увагу** Ви можете ігнорувати будь-яку сторінку веб-браузера, відкриту до веб-сайту TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="cb187-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="cb187-123">Визначи запит на додаток TeamViewer для внесення змін до пристрою (лише для Windows).</span><span class="sxs-lookup"><span data-stu-id="cb187-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="cb187-124">Застосунок TeamViewer запускається та містить код сеансу для автентифікації підключення до віддаленого пристрою.</span><span class="sxs-lookup"><span data-stu-id="cb187-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="cb187-125">Спливаюче запитує, якщо ви хочете дозволити початку сесії.</span><span class="sxs-lookup"><span data-stu-id="cb187-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="cb187-126">**Зверніть увагу** Коди сеансів, створені службою TeamViewer, є лише одним часом використання.</span><span class="sxs-lookup"><span data-stu-id="cb187-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="cb187-127">Якщо ви втратите з'єднання, ви повинні:</span><span class="sxs-lookup"><span data-stu-id="cb187-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="cb187-128">Закрийте екземпляр програми TeamViewer на віддаленому пристрої та на робочій станції адміністратора.</span><span class="sxs-lookup"><span data-stu-id="cb187-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="cb187-129">Закрийте портал компанії на віддаленому пристрої.</span><span class="sxs-lookup"><span data-stu-id="cb187-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="cb187-130">Запустіть нову "новий сеанс віддаленої допомоги" з порталу адміністратора.</span><span class="sxs-lookup"><span data-stu-id="cb187-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="cb187-131">Відкрийте портал компанії на віддаленому пристрої, щоб отримати нове сповіщення.</span><span class="sxs-lookup"><span data-stu-id="cb187-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="cb187-132">Завантажте та відкрийте програму TeamViewer на віддаленому пристрої та робочій станції адміністратора, як і раніше.</span><span class="sxs-lookup"><span data-stu-id="cb187-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>