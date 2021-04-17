---
title: Перенесення З AIP на MIP/Unified Labeling у Центрі відповідності
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825392"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="c5938-102">Перенесення З AIP на MIP/Unified Labeling у Центрі відповідності</span><span class="sxs-lookup"><span data-stu-id="c5938-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="c5938-103">Щоб перенести з етикеток AIP до пункту Уніфіковане підписування в Центрі безпеки та відповідності, виконайте такі дії:</span><span class="sxs-lookup"><span data-stu-id="c5938-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="c5938-104">**Активація захисту з порталу Azure**</span><span class="sxs-lookup"><span data-stu-id="c5938-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="c5938-105">Якщо ви цього ще не зробили, відкрийте нове вікно браузера та [ввійдіть на портал Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="c5938-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="c5938-106">Перейдіть до **лотка "Захист** даних в Azure".</span><span class="sxs-lookup"><span data-stu-id="c5938-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="c5938-107">Наприклад, у меню Центр клацніть  Усі служби та почніть **вводити** дані в полі Фільтр.</span><span class="sxs-lookup"><span data-stu-id="c5938-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="c5938-108">Виберіть **Захист даних в Azure**.</span><span class="sxs-lookup"><span data-stu-id="c5938-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="c5938-109">Якщо ви раніше не отримували доступу до полотна "Захист [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) даних в Azure", див. одноразові додаткові дії з додавання цього блоку до порталу.</span><span class="sxs-lookup"><span data-stu-id="c5938-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="c5938-110">Щоб відкрити ледь захист даних в Azure, потрібно мати план [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) або план Office 365, який включає керування правами.</span><span class="sxs-lookup"><span data-stu-id="c5938-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="c5938-111">Якщо у вас є одна з цих передплат, але відображається повідомлення про те, що не вдалося знайти дійсну передплату, зверніться до служби підтримки [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) або скористайтеся стандартними каналами підтримки.</span><span class="sxs-lookup"><span data-stu-id="c5938-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="c5938-112">Знайдіть **параметри меню Керування** та виберіть Захист **активація**.</span><span class="sxs-lookup"><span data-stu-id="c5938-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="c5938-113">Натисніть **кнопку Активувати,** а потім підтвердьте дію.</span><span class="sxs-lookup"><span data-stu-id="c5938-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="c5938-114">Коли активацію завершено, інформаційний рядок відображає вікно **Активацію успішно завершено.**</span><span class="sxs-lookup"><span data-stu-id="c5938-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="c5938-115">**Перенесення етикеток захисту даних Azure до Центру безпеки & Office 365**</span><span class="sxs-lookup"><span data-stu-id="c5938-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="c5938-116">Переконайтеся, що ви ввійшли як користувач із дозволом глобального адміністратора.</span><span class="sxs-lookup"><span data-stu-id="c5938-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="c5938-117">Перейдіть до **лотка "Захист** даних в Azure".</span><span class="sxs-lookup"><span data-stu-id="c5938-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="c5938-118">У меню **"Керування"** виберіть пункт **Уніфіковане підписування**.</span><span class="sxs-lookup"><span data-stu-id="c5938-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="c5938-119">У **засобі "Захист даних в Azure – уніфікований надпис"** натисніть кнопку **Активувати** та дотримуйтеся вказівок в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="c5938-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="c5938-120">**Примітка.** Перш ніж активувати перенесення Центру відповідності &, переконайтеся, що у вас є відповідні дозволи.</span><span class="sxs-lookup"><span data-stu-id="c5938-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="c5938-121">Докладні відомості див. в цих статтях:</span><span class="sxs-lookup"><span data-stu-id="c5938-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="c5938-122">Чи потрібно вам глобальним адміністратором настроювати захист даних в Azure або делегувати іншим адміністраторам?</span><span class="sxs-lookup"><span data-stu-id="c5938-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="c5938-123">Важлива інформація про адміністративні ролі після перенесення до Центру безпеки & відповідності.</span><span class="sxs-lookup"><span data-stu-id="c5938-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="c5938-124">Докладні відомості про AIP до Центру безпеки та відповідності див. в цьому [центрі.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="c5938-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
