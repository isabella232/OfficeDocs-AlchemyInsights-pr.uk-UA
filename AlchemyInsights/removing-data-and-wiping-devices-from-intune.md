---
title: Видалення даних і витираючи пристроїв з InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440462"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="cd9a5-102">Видалення даних і витираючи пристроїв з InTune</span><span class="sxs-lookup"><span data-stu-id="cd9a5-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="cd9a5-103">Пристрій на пенсію і пристрій стирання віддалених дій можна використовувати для видалення даних компанії, які керуються InTune або виконати Скидання заводських налаштувань і повернути пристрій до настройок за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="cd9a5-104">Увійдіть до Microsoft 365 керування пристроями та перейдіть до **пристроїв**на  >  **всіх пристроях**.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="cd9a5-105">Виберіть пристрій, який потрібно стерти.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="cd9a5-106">Виберіть тип віддаленого стирання, яку потрібно виконати.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="cd9a5-107">На пенсію видаляються лише організаційні відомості, а повні серветки відновлюють пристрій до заводських налаштувань.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="cd9a5-108">Виберіть **так** , щоб підтвердити.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="cd9a5-109">До стирання завершиться, стан дії пристрою відображається як пенсію очікування.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="cd9a5-110">Після завершення дії ви більше не побачите мобільного пристрою у списку керованих пристроїв.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="cd9a5-111">**Зверніть увагу** Дані компанії не можна видалити з пристроїв, які ПРИЄДНАЛИСЯ до Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cd9a5-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="cd9a5-112">Щоб отримати докладні відомості про дію на пенсію і стерти дії, у тому числі те, що зберігається і що видаляється, див [видалення пристроїв за допомогою стирання, пенсію або вручну, скасування реєстрації пристрою](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="cd9a5-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="cd9a5-113">Щоб стерти всі дані з пристрою macOS, перегляньте цю інформацію [з пристрою MacOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="cd9a5-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>