---
title: Offboard непристроїв із Windows від засобу захисту від досвідчених загроз Microsoft Defender (АТФ)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748487"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="56da9-102">Offboard непристроїв із Windows від засобу захисту від досвідчених загроз Microsoft Defender (АТФ)</span><span class="sxs-lookup"><span data-stu-id="56da9-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="56da9-103">Ось як це зробити.</span><span class="sxs-lookup"><span data-stu-id="56da9-103">Here's how:</span></span>

1. <span data-ttu-id="56da9-104">Виконайте документацію третьої сторони, щоб від'єднатися від стороннього рішення від компанії Microsoft Defender АТФ.</span><span class="sxs-lookup"><span data-stu-id="56da9-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="56da9-105">З клієнта Azure Active Directory, видаліть дозволи для рішення стороннього виробника.</span><span class="sxs-lookup"><span data-stu-id="56da9-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="56da9-106">Увійдіть на [портал Azure](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="56da9-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="56da9-107">Виберіть **Усі служби**"  >  **блакитні активні каталоги**" для  >  **корпоративних програм**.</span><span class="sxs-lookup"><span data-stu-id="56da9-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="56da9-108">Виберіть програму, яку потрібно додати до offboard.</span><span class="sxs-lookup"><span data-stu-id="56da9-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="56da9-109">Натисніть кнопку **Видалити**.</span><span class="sxs-lookup"><span data-stu-id="56da9-109">Select **Delete**.</span></span>

<span data-ttu-id="56da9-110">Докладні відомості можна знайти в [надбудові offboard, що не є пристроями для Windows](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="56da9-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
