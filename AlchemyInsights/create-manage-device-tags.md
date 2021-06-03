---
title: Створення тегів або груп пристроїв і керування ними
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731972"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="60180-102">Створення тегів або груп пристроїв і керування ними</span><span class="sxs-lookup"><span data-stu-id="60180-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="60180-103">Додайте позначки на пристроях, щоб створити зв'язку в логічній групі.</span><span class="sxs-lookup"><span data-stu-id="60180-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="60180-104">Позначки пристроїв підтримують правильне зіставлення мережі, що дає змогу прикріпити різні позначки для записування контексту та активувати динамічне створення списку в складі інциденту.</span><span class="sxs-lookup"><span data-stu-id="60180-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="60180-105">Позначки можна використовувати як фільтр у поданні списку "Пристрої" або групувати пристрої.</span><span class="sxs-lookup"><span data-stu-id="60180-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="60180-106">Докладні відомості про групування пристроїв див. в розділі [Створення тегів пристроїв і керування ними.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="60180-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="60180-107">Теги можна додавати на пристроях:</span><span class="sxs-lookup"><span data-stu-id="60180-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="60180-108">Використання порталу</span><span class="sxs-lookup"><span data-stu-id="60180-108">Using the portal</span></span>

- <span data-ttu-id="60180-109">Настроювання значення розділу реєстру</span><span class="sxs-lookup"><span data-stu-id="60180-109">Setting a registry key value</span></span>
 
<span data-ttu-id="60180-110">**Примітка.** Можливо, між часом додавання позначки до пристрою та його доступністю в списку пристроїв і на сторінці пристрою може виникати затримка.</span><span class="sxs-lookup"><span data-stu-id="60180-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="60180-111">Щоб дізнатися, як додати позначки пристроїв за допомогою API, див. номери Додавання та видалення [API-тегів пристроїв.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="60180-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="60180-112">Додавання тегів пристроїв і керування ними за допомогою порталу</span><span class="sxs-lookup"><span data-stu-id="60180-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="60180-113">Виберіть пристрій, на якому потрібно керувати позначками.</span><span class="sxs-lookup"><span data-stu-id="60180-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="60180-114">Ви можете вибрати або знайти пристрій у будь-якому з таких подань:</span><span class="sxs-lookup"><span data-stu-id="60180-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="60180-115">**Приладна дошка операцій безпеки** Виберіть ім'я пристрою в розділі Найпопулярніші пристрої з активними оповіщеннями.</span><span class="sxs-lookup"><span data-stu-id="60180-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="60180-116">**Черга оповіщень–** виберіть ім'я пристрою поруч із піктограмою пристрою в черзі оповіщень.</span><span class="sxs-lookup"><span data-stu-id="60180-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="60180-117">**Список Пристрої** – виберіть ім'я пристрою зі списку пристроїв.</span><span class="sxs-lookup"><span data-stu-id="60180-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="60180-118">**Поле пошуку.** У розкривному меню виберіть пункт Пристрій і введіть ім'я пристрою.</span><span class="sxs-lookup"><span data-stu-id="60180-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="60180-119">Сторінку оповіщення також можна відкрити в поданнях файлів і IP-адрес.</span><span class="sxs-lookup"><span data-stu-id="60180-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="60180-120">У **рядку Дій** із відповіддю виберіть керування позначками.</span><span class="sxs-lookup"><span data-stu-id="60180-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="60180-121">Введіть, щоб знайти або створити позначки.</span><span class="sxs-lookup"><span data-stu-id="60180-121">Type to find or create tags.</span></span>

<span data-ttu-id="60180-122">Позначки додаються до подання пристрою та відображаються в поданні списку Пристрої.</span><span class="sxs-lookup"><span data-stu-id="60180-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="60180-123">Потім можна скористатися фільтром "Позначки", щоб переглянути відповідний список пристроїв.</span><span class="sxs-lookup"><span data-stu-id="60180-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="60180-124">Докладні відомості див. в [розділі Створення позначок пристроїв і керування ними.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="60180-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>