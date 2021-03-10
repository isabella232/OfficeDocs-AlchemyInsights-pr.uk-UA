---
title: Виправлення політики підключення
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695892"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="bc93b-102">Виправлення політики підключення</span><span class="sxs-lookup"><span data-stu-id="bc93b-102">Fix connection policy</span></span>

<span data-ttu-id="bc93b-103">Повідомлення електронної пошти було позначено безпечним і доставлено в папку "Вхідні" користувача, оскільки IP-адреса, що надсилається, була позначена в політиці фільтра підключення.</span><span class="sxs-lookup"><span data-stu-id="bc93b-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="bc93b-104">Щоб переглянути політику, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="bc93b-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="bc93b-105">Перейдіть до [центру відповідності & безпеки Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143), а потім перейдіть до політики **керування загрозою**"  >    >  [Anti-спаму](https://go.microsoft.com/fwlink/?linkid=2101518)".</span><span class="sxs-lookup"><span data-stu-id="bc93b-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="bc93b-106">На вкладці **Додатково** виберіть **політику фільтра підключення**, а потім натисніть кнопку **редагувати політику**.</span><span class="sxs-lookup"><span data-stu-id="bc93b-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="bc93b-107">Перегляньте список **дозволених IP-адрес** .</span><span class="sxs-lookup"><span data-stu-id="bc93b-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="bc93b-108">Перевірте, чи ввімкнуто **безпечний список** .</span><span class="sxs-lookup"><span data-stu-id="bc93b-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="bc93b-109">Корпорація Майкрософт приєднується до джерел третьої сторони надійних відправників.</span><span class="sxs-lookup"><span data-stu-id="bc93b-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="bc93b-110">Якщо ввімкнуто **безпечний список** , ці Надійні відправники не позначаються як спам.</span><span class="sxs-lookup"><span data-stu-id="bc93b-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="bc93b-111">Я рекомендую вибрати цей параметр, оскільки він зменшить кількість помилкових спрацьовувань (вдала пошта, класифікована як спам), що ви отримуєте.</span><span class="sxs-lookup"><span data-stu-id="bc93b-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
