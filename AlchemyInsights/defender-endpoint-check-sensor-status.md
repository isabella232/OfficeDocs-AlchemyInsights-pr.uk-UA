---
title: Кінцева точка Захисника перевірити стан датчика
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676544"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="08492-102">Кінцева точка Захисника перевірити стан датчика</span><span class="sxs-lookup"><span data-stu-id="08492-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="08492-103">Плитка **Пристрої з проблемами датчика** міститься на приладні дошці "Операції безпеки".</span><span class="sxs-lookup"><span data-stu-id="08492-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="08492-104">Ця плитка містить відомості про можливість окремого пристрою надавати дані датчиків і спілкуватися зі службою "Захисник кінцевих точок".</span><span class="sxs-lookup"><span data-stu-id="08492-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="08492-105">У ньому повідомляється, скільки пристроїв потребує уваги, і допоможе виявити проблемні пристрої та вживати заходів для виправлення відомих проблем.</span><span class="sxs-lookup"><span data-stu-id="08492-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="08492-106">На плитці міститься інформація про кількість пристроїв, які не повідомляли належним чином для служби:</span><span class="sxs-lookup"><span data-stu-id="08492-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="08492-107">**Неправильно настроєний** Пристрої, на яких може бути частково повідомлено дані датчиків до служби "Захисник" для служби кінцевих точок, і можуть виникати помилки конфігурації, які потрібно виправити.</span><span class="sxs-lookup"><span data-stu-id="08492-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="08492-108">**Неактивний** Пристрої, які припинили звітування в службу "Захисник" для служби кінцевих точок більше семи днів за останній місяць.</span><span class="sxs-lookup"><span data-stu-id="08492-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="08492-109">Клацнувши будь-яку групу, можна вибрати список Пристрої, відфільтрований відповідно до вибраних варіантів.</span><span class="sxs-lookup"><span data-stu-id="08492-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="08492-110">У списку Пристрої можна відфільтрувати список станів справності за таким станом:</span><span class="sxs-lookup"><span data-stu-id="08492-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="08492-111">**Активний** Пристрої, які активно повідомляють Захиснику служби кінцевих точок.</span><span class="sxs-lookup"><span data-stu-id="08492-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="08492-112">**Неправильно настроєний** Пристрої, які можуть частково повідомляти про дані датчиків для служби "Захисник кінцевих точок", але мають помилки конфігурації, які потрібно виправити.</span><span class="sxs-lookup"><span data-stu-id="08492-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="08492-113">Неправильно настроєні пристрої можуть мати один або кілька таких проблем:</span><span class="sxs-lookup"><span data-stu-id="08492-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="08492-114">Жодних даних датчиків – Пристрої припинили надсилати дані датчиків.</span><span class="sxs-lookup"><span data-stu-id="08492-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="08492-115">На пристрої можна отримувати обмежені оповіщення.</span><span class="sxs-lookup"><span data-stu-id="08492-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="08492-116">Порушення зв'язку – порушення зв'язку з пристроєм.</span><span class="sxs-lookup"><span data-stu-id="08492-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="08492-117">Надсилання файлів для глибокого аналізу, блокування файлів, ізоляція пристрою з мережі та інших дій, які вимагають зв'язку з пристроєм, можуть не працювати.</span><span class="sxs-lookup"><span data-stu-id="08492-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="08492-118">**Неактивний** Пристрої, які припинили звітування для служби кінцевих точок Захисника.</span><span class="sxs-lookup"><span data-stu-id="08492-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="08492-119">За допомогою функції експорту можна завантажити весь список у форматі CSV.</span><span class="sxs-lookup"><span data-stu-id="08492-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="08492-120">Докладні відомості див. в статті [Перевірка стану справності датчика в Microsoft Defender для кінцевої точки.](/microsoft-365/security/defender-endpoint/check-sensor-status)</span><span class="sxs-lookup"><span data-stu-id="08492-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="08492-121">Докладні відомості про те, що спричинило неактивний або неправильно настроєний пристрій, див. в статті Виправлення несправних датчиків у Microsoft [Defender для кінцевої точки.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="08492-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
