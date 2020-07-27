---
title: Обхід блокування активації на контрольованих пристроях iOS з InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424208"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="7d745-102">Обхід блокування активації на контрольованих пристроях iOS з InTune</span><span class="sxs-lookup"><span data-stu-id="7d745-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="7d745-103">Можливість обійти блокування активації на пристроях iOS полегшує відновлення за сценарієм, коли користувач активує блокування активації на корпоративному пристрої, а потім залишає компанію.</span><span class="sxs-lookup"><span data-stu-id="7d745-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="7d745-104">Передумови для обходу блокування активації включають:</span><span class="sxs-lookup"><span data-stu-id="7d745-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="7d745-105">Пристрій, що "контролюється".</span><span class="sxs-lookup"><span data-stu-id="7d745-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="7d745-106">Блокування активації успішно ввімкнуто, використовуючи iOS пристрою обмеження політики в InTune.</span><span class="sxs-lookup"><span data-stu-id="7d745-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="7d745-107">Крім того, при минаючи блокування активації вам необхідно:</span><span class="sxs-lookup"><span data-stu-id="7d745-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="7d745-108">Фізично володіти пристроєм, що знищили.</span><span class="sxs-lookup"><span data-stu-id="7d745-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="7d745-109">Скопіюйте код, перш ніж видати стирання.</span><span class="sxs-lookup"><span data-stu-id="7d745-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="7d745-110">**Примітка:** Код стирання не чутливий до регістру, тому символи "-" не потрібні.</span><span class="sxs-lookup"><span data-stu-id="7d745-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="7d745-111">Докладні відомості наведено в [обхід блокування активації на контрольованих пристроях IOS із InTune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="7d745-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="7d745-112">**Запитання й відповіді**</span><span class="sxs-lookup"><span data-stu-id="7d745-112">**FAQ**</span></span>

<span data-ttu-id="7d745-113">Q: **я видав віддалену дію, щоб видалити дані компанії з пристрою, і тепер він застряг у стані очікування.**</span><span class="sxs-lookup"><span data-stu-id="7d745-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="7d745-114">В: для віддаленої дії, щоб успішно завершити, цільовий пристрій повинен бути онлайн і здоровим.</span><span class="sxs-lookup"><span data-stu-id="7d745-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="7d745-115">У таких ситуаціях Віддалена дія залишається в стані очікування протягом 30 днів або поки пристрій не визнає команду, коли пристрій:</span><span class="sxs-lookup"><span data-stu-id="7d745-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="7d745-116">Не має підключення.</span><span class="sxs-lookup"><span data-stu-id="7d745-116">Does not have connectivity.</span></span>
- <span data-ttu-id="7d745-117">Втрачає статус керування з InTune.</span><span class="sxs-lookup"><span data-stu-id="7d745-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="7d745-118">Якщо ви вважаєте, що пристрій більше не перевірятися, і що він не видаляє дані компанії, виберіть Видалити.</span><span class="sxs-lookup"><span data-stu-id="7d745-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="7d745-119">Видалення видаляє запис пристрою так, що він більше не відображається у списку InTune пристроїв.</span><span class="sxs-lookup"><span data-stu-id="7d745-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="7d745-120">Щоб пристрій став активним знову, його користувач повинен повторно зареєструвати пристрій.</span><span class="sxs-lookup"><span data-stu-id="7d745-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="7d745-121">П: **чому деякі віддалені дії недоступні для мене?**</span><span class="sxs-lookup"><span data-stu-id="7d745-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="7d745-122">В: не всі платформи підтримують всі дії з віддаленим пристроєм.</span><span class="sxs-lookup"><span data-stu-id="7d745-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="7d745-123">Такі віддалені дії є специфічними для платформи.</span><span class="sxs-lookup"><span data-stu-id="7d745-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="7d745-124">Обхід блокування активації (лише для iOS)</span><span class="sxs-lookup"><span data-stu-id="7d745-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="7d745-125">Чистий запуск (лише для Windows)</span><span class="sxs-lookup"><span data-stu-id="7d745-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="7d745-126">Втрачений режим (лише для iOS)</span><span class="sxs-lookup"><span data-stu-id="7d745-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="7d745-127">Пошук пристрою (лише для iOS)</span><span class="sxs-lookup"><span data-stu-id="7d745-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="7d745-128">Перезапустити (лише для Windows)</span><span class="sxs-lookup"><span data-stu-id="7d745-128">Restart (Windows only)</span></span>

<span data-ttu-id="7d745-129">Щоб отримати докладніші відомості про кожну дію, перегляньте [доступні дії пристрою](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="7d745-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>