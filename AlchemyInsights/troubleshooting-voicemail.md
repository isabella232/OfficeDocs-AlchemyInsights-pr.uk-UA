---
title: 'Виправлення неполадок голосової пошти '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679108"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="b3479-102">Виправлення неполадок голосової пошти</span><span class="sxs-lookup"><span data-stu-id="b3479-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="b3479-103">Переконайтеся, що для функції "зайнятий зайнятий" виконується навмисне.</span><span class="sxs-lookup"><span data-stu-id="b3479-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="b3479-104">Якщо ця функція не потрібна для цього користувача, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="b3479-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="b3479-105">Перейдіть до [центру адміністрування команд](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="b3479-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="b3479-106">У лівій залізничній області Навігація політики **голосового** зв'язку  >    >  **керуватимуть політиками** в **політиці виклику**.</span><span class="sxs-lookup"><span data-stu-id="b3479-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="b3479-107">Виберіть елемент **керування користувачами**.</span><span class="sxs-lookup"><span data-stu-id="b3479-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="b3479-108">Знайдіть користувача та змініть політику викликів, яку **зайнятий на зайнятий, коли під час виклику** **.**</span><span class="sxs-lookup"><span data-stu-id="b3479-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="b3479-109">Натисніть кнопку **Застосувати**.</span><span class="sxs-lookup"><span data-stu-id="b3479-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="b3479-110">Зміни в політиці можуть знадобитися до 24 годин, щоб реплікувати.</span><span class="sxs-lookup"><span data-stu-id="b3479-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="b3479-111">Щоб отримати докладніші відомості про цю функцію: [зайнятий зайнятий, доступний під час виклику](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="b3479-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>
