---
title: Inune для інвентаризації пристрою
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
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667899"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="90fee-102">Inune для інвентаризації пристрою</span><span class="sxs-lookup"><span data-stu-id="90fee-102">Intune Device Inventory</span></span>

<span data-ttu-id="90fee-103">Лезо "пристрої" надає адміністратору доступ до пристроїв у розділі "керування" на основі для кожного пристрою.</span><span class="sxs-lookup"><span data-stu-id="90fee-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="90fee-104">Відомості, що відображаються: Устаткування, виявлено програми, стан відповідності пристрою та стан конфігурації пристрою.</span><span class="sxs-lookup"><span data-stu-id="90fee-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="90fee-105">Дані інвентарного списку для обладнання та виявлених програм зібрані за семиденний цикл.</span><span class="sxs-lookup"><span data-stu-id="90fee-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="90fee-106">Програми та окремі елементи обладнання, що повідомляються, залежать від операційної системи пристрою, а також про те, чи є пристрій особистою чи корпоративною.</span><span class="sxs-lookup"><span data-stu-id="90fee-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="90fee-107">Докладні відомості наведено [в статті Перегляд відомостей про пристрій у програмі Inune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="90fee-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="90fee-108">**Запитання й відповіді**</span><span class="sxs-lookup"><span data-stu-id="90fee-108">**FAQ**</span></span>

<span data-ttu-id="90fee-109">П: я не отримую повний перелік програм, які присутні на пристроях із Windows.</span><span class="sxs-lookup"><span data-stu-id="90fee-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="90fee-110">Чому ні?</span><span class="sxs-lookup"><span data-stu-id="90fee-110">Why not?</span></span>

<span data-ttu-id="90fee-111">В: цього разу доступні лише сучасні програми, які перелічено для ПК з Windows 10, виявлених як корпоративні пристрої.</span><span class="sxs-lookup"><span data-stu-id="90fee-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="90fee-112">Inune не збирає відомості про програми Win32, інстальовані на цих пристроях.</span><span class="sxs-lookup"><span data-stu-id="90fee-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="90fee-113">Запитання: чому телефонні номери не зібрані з усіх пристроїв?</span><span class="sxs-lookup"><span data-stu-id="90fee-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="90fee-114">В: телефони, які класифікуються як корпоративні пристрої в Inune, не ідентифіковано за допомогою свого повного номера телефону, коли, наприклад, ви запускаєте звіт про інвентаризацію мобільного пристрою.</span><span class="sxs-lookup"><span data-stu-id="90fee-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="90fee-115">Усі номери телефонів із власними пристроями завжди частково маскуються за допомогою зірочки (\* \* \* \*) і відображаються лише останні чотири цифри.</span><span class="sxs-lookup"><span data-stu-id="90fee-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>