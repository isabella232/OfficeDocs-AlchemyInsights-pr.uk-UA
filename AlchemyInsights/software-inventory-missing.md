---
title: Відсутні або неточні запаси програмного забезпечення
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676587"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="0b97b-102">Відсутні або неточні запаси програмного забезпечення</span><span class="sxs-lookup"><span data-stu-id="0b97b-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="0b97b-103">Інвентарний список програмного забезпечення керування загрозами та вразливостями (TVM) – це список відомих програм у вашій організації, де офіційно використовується офіційне перелічення платформи (CPE).</span><span class="sxs-lookup"><span data-stu-id="0b97b-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="0b97b-104">Програмні продукти без офіційного засобу CPE не публікують вразливості.</span><span class="sxs-lookup"><span data-stu-id="0b97b-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="0b97b-105">Крім того, цей інвентарний список містить такі відомості, як ім'я постачальника, кількість слабких частин, загроз і кількість підключених пристроїв.</span><span class="sxs-lookup"><span data-stu-id="0b97b-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="0b97b-106">Зміни програмного забезпечення на пристроях зазвичай відображаються на порталах безпеки протягом двох годин.</span><span class="sxs-lookup"><span data-stu-id="0b97b-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="0b97b-107">Проте інколи це може зайняти більше часу.</span><span class="sxs-lookup"><span data-stu-id="0b97b-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="0b97b-108">Наразі не можна примусово синхронізувати дані. це поточна безперервна оцінювання.</span><span class="sxs-lookup"><span data-stu-id="0b97b-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="0b97b-109">Якщо ви внесли зміни до програмного забезпечення та зміни не відображаються на телевізійному каналі через 5 годин, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="0b97b-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="0b97b-110">Перегляньте розділ доказів програмного забезпечення, щоб дізнатися, як виявлено програмне забезпечення.</span><span class="sxs-lookup"><span data-stu-id="0b97b-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="0b97b-111">Переконайтеся, що програмне забезпечення підтримується.</span><span class="sxs-lookup"><span data-stu-id="0b97b-111">Make sure that the software is supported.</span></span> <span data-ttu-id="0b97b-112">Програмне забезпечення може відображатися лише на рівні пристрою, навіть якщо воно наразі не підтримується керування загрозами та вразливостями.</span><span class="sxs-lookup"><span data-stu-id="0b97b-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="0b97b-113">Проте доступно лише обмежені дані.</span><span class="sxs-lookup"><span data-stu-id="0b97b-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="0b97b-114">Кроки зі звітування про неточність на порталі див. в статті Повідомлення про [неточність.](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)</span><span class="sxs-lookup"><span data-stu-id="0b97b-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="0b97b-115">**Примітка.** Повідомлення про неточність з порталу MDE – це односхідний канал проектування.</span><span class="sxs-lookup"><span data-stu-id="0b97b-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="0b97b-116">Якщо ця проблема терміново виникає, надішлюйте запит на підтримку.</span><span class="sxs-lookup"><span data-stu-id="0b97b-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="0b97b-117">Докладні відомості [див. в цій](/microsoft-365/security/defender-endpoint/tvm-software-inventory)керування загрозами та вразливостями.</span><span class="sxs-lookup"><span data-stu-id="0b97b-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>