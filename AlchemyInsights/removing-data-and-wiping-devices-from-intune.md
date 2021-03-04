---
title: Видалення даних та стирання пристроїв з Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416334"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="cad2a-102">Видалення даних та стирання пристроїв з Intune</span><span class="sxs-lookup"><span data-stu-id="cad2a-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="cad2a-103">Віддалені дії "Списання пристрою" і "Стирання пристрою" можуть бути використані для видалення даних організації, якими керує Intune, або для скидання до заводських налаштувань та повернення пристрою до налаштувань за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="cad2a-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="cad2a-104">Увійдіть на інформаційну панель "Керування пристроями в Microsoft 365" та перейдіть у розділ **Пристрої** > **Усі пристрої**.</span><span class="sxs-lookup"><span data-stu-id="cad2a-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="cad2a-105">Виберіть пристрій, який необхідно стерти.</span><span class="sxs-lookup"><span data-stu-id="cad2a-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="cad2a-106">Виберіть тип віддаленого стирання.</span><span class="sxs-lookup"><span data-stu-id="cad2a-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="cad2a-107">Списання видаляє лише організаційну інформацію, а повне стирання відновлює пристрій до заводських налаштувань.</span><span class="sxs-lookup"><span data-stu-id="cad2a-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="cad2a-108">Натисніть кнопку **Так** для підтвердження.</span><span class="sxs-lookup"><span data-stu-id="cad2a-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="cad2a-109">Поки стирання не завершиться, у статусі дії пристрою відображатиметься *Триває списання*.</span><span class="sxs-lookup"><span data-stu-id="cad2a-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="cad2a-110">Після завершення дії ви більше не бачитимете мобільний пристрій у списку керованих.</span><span class="sxs-lookup"><span data-stu-id="cad2a-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="cad2a-111">Дані організації не можна видалити з пристроїв, ПРИЄДНАНИХ до Microsoft Azure AD.</span><span class="sxs-lookup"><span data-stu-id="cad2a-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="cad2a-112">Повну інформацію про ефект дій "Списати" та "Стерти", зокрема те, що збережено та що видалено, див. у таких документах:</span><span class="sxs-lookup"><span data-stu-id="cad2a-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="cad2a-113">[Видалення пристроїв за допомогою функцій стирання, списання або відключення пристрою вручну](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="cad2a-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="cad2a-114">Як видалити лише корпоративні дані з керованих Intune програм</span><span class="sxs-lookup"><span data-stu-id="cad2a-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="cad2a-115">[Видалення всіх даних із пристрою macOS](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="cad2a-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>