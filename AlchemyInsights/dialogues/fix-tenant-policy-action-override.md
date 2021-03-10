---
title: Виправлення політики клієнта (перевизначення дії)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695689"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="2e55e-102">Виправлення політики клієнта (перевизначення дії)</span><span class="sxs-lookup"><span data-stu-id="2e55e-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="2e55e-103">Це повідомлення вплине на політику захисту від спаму в клієнті.</span><span class="sxs-lookup"><span data-stu-id="2e55e-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="2e55e-104">Щоб переглянути політику, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="2e55e-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="2e55e-105">Перейдіть до [центру відповідності & безпеки Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), а потім перейдіть до політики **керування загрозою**"  >    >  [Anti-спаму](https://go.microsoft.com/fwlink/?linkid=2101518)".</span><span class="sxs-lookup"><span data-stu-id="2e55e-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="2e55e-106">Перевірте, чи є **джерело політики** , що вказує на таке:  **Add-XHeader/Momesfyтема/переспрямування та видалення/без дій і прихованої копії повідомлення**</span><span class="sxs-lookup"><span data-stu-id="2e55e-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="2e55e-107">Якщо так, на вкладці **Додатково** установіть прапорець настройки політики, які вплинули на повідомлення.</span><span class="sxs-lookup"><span data-stu-id="2e55e-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="2e55e-108">Можливо, **стандартні параметри** , застосовані до всіх клієнтів Exchange Online Protection, вплинули на повідомлення.</span><span class="sxs-lookup"><span data-stu-id="2e55e-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="2e55e-109">Докладні відомості про настроювання політик фільтрування спаму наведено в статті [Настроювання політик фільтра спаму](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="2e55e-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
