---
title: Проблеми з видаленням з'єднуваного або дезахизаційного пристрою з інвентарного списку пристроїв
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564613"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="6fa8f-102">Проблеми з видаленням з'єднуваного або дезахизаційного пристрою з інвентарного списку пристроїв</span><span class="sxs-lookup"><span data-stu-id="6fa8f-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="6fa8f-103">Захисник Microsoft для кінцевої точки наразі не дозволяє вручну видалити запис пристрою з адаптивного або декомпіляційного пристрою з інвентарного списку пристроїв.</span><span class="sxs-lookup"><span data-stu-id="6fa8f-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="6fa8f-104">З міркуваннями безпеки пристрій залишається на порталі як історичний запис протягом 180 днів.</span><span class="sxs-lookup"><span data-stu-id="6fa8f-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="6fa8f-105">Проте дані пристрою одужуються відповідно до налаштованого періоду збереження.</span><span class="sxs-lookup"><span data-stu-id="6fa8f-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="6fa8f-106">**Примітка.** Після семи днів адаптивний пристрій автоматично переключиться на **неактивний** стан.</span><span class="sxs-lookup"><span data-stu-id="6fa8f-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="6fa8f-107">Крім того, дані, які відображають оцінку виставлення рахунку або Microsoft Secure Score для пристроїв, не впливають на пристрої за останні 30 днів, не впливають на дані, які керування загрозами та вразливостями оцінку виставлення рахунку або Microsoft Secure Score.</span><span class="sxs-lookup"><span data-stu-id="6fa8f-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="6fa8f-108">Якщо ви все одно не хочете бачити певні пристрої в поданні інвентарного списку пристроїв, спробуйте розмістити тег пристрою, щоб відфільтрувати знятий пристрій із подання "Запаси пристроїв".</span><span class="sxs-lookup"><span data-stu-id="6fa8f-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="6fa8f-109">Докладні відомості:</span><span class="sxs-lookup"><span data-stu-id="6fa8f-109">For more information, see:</span></span>

[<span data-ttu-id="6fa8f-110">З'єднувачі зі служби кінцевих точок Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="6fa8f-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="6fa8f-111">Оцінка експозиції в керування загрозами та вразливостями</span><span class="sxs-lookup"><span data-stu-id="6fa8f-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="6fa8f-112">Виправлення незмінних датчиків у Microsoft Defender для кінцевої точки</span><span class="sxs-lookup"><span data-stu-id="6fa8f-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="6fa8f-113">Ефективне використання тегів (частина 1)</span><span class="sxs-lookup"><span data-stu-id="6fa8f-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="6fa8f-114">Ефективне використання тегів (частина 2)</span><span class="sxs-lookup"><span data-stu-id="6fa8f-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="6fa8f-115">Ефективне використання тегів (частина 3)</span><span class="sxs-lookup"><span data-stu-id="6fa8f-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




