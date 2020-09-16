---
title: Перенесення з AIP до MIP/уніфікованого маркування в центрі відповідності
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674347"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="4334b-102">Перенесення з AIP до MIP/уніфікованого маркування в центрі відповідності</span><span class="sxs-lookup"><span data-stu-id="4334b-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="4334b-103">Щоб перенести з міток AIP до уніфікованого маркування в центрі безпеки та відповідності, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="4334b-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="4334b-104">**Активація захисту від порталу "Лазурний"**</span><span class="sxs-lookup"><span data-stu-id="4334b-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="4334b-105">Якщо ви ще не зробили цього, відкрийте нове вікно браузера та [ввійдіть на порталі Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="4334b-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="4334b-106">Перейдіть на відповідне лезо для **захисту інформації** .</span><span class="sxs-lookup"><span data-stu-id="4334b-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="4334b-107">Наприклад, у меню "концентратор" виберіть пункт **Усі служби** та починайте вводити **дані** в полі фільтра.</span><span class="sxs-lookup"><span data-stu-id="4334b-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="4334b-108">Виберіть пункт **захист інформації з Azure**.</span><span class="sxs-lookup"><span data-stu-id="4334b-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="4334b-109">Якщо ви ще не отримували відповідь на захист інформації в Лазурне, перегляньте один раз [додаткові кроки](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , щоб додати цей Клинок до порталу.</span><span class="sxs-lookup"><span data-stu-id="4334b-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="4334b-110">Щоб відкрити відповідний елемент захисту від Блакитної інформації, необхідно мати [або план](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) Office 365, який включає в себе керування правами.</span><span class="sxs-lookup"><span data-stu-id="4334b-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="4334b-111">Якщо у вас є одна з цих передплат, але відображається повідомлення про те, що дійсна Передплата не знайдена, [зверніться до служби підтримки Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) або скористайтеся стандартними каналами підтримки.</span><span class="sxs-lookup"><span data-stu-id="4334b-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="4334b-112">Знайдіть пункти меню **керування** , а потім виберіть пункт **Активація захисту**.</span><span class="sxs-lookup"><span data-stu-id="4334b-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="4334b-113">Натисніть кнопку **активувати**, а потім підтвердьте дію.</span><span class="sxs-lookup"><span data-stu-id="4334b-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="4334b-114">Після завершення активації інформаційна панель відображає **активацію успішно завершено**.</span><span class="sxs-lookup"><span data-stu-id="4334b-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="4334b-115">**Перенесення міток захисту даних Azure до центру відповідності & безпеки Office 365**</span><span class="sxs-lookup"><span data-stu-id="4334b-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="4334b-116">Переконайтеся, що ви ввійшли як користувач із дозволом глобального адміністратора.</span><span class="sxs-lookup"><span data-stu-id="4334b-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="4334b-117">Перейдіть на відповідне лезо для **захисту інформації** .</span><span class="sxs-lookup"><span data-stu-id="4334b-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="4334b-118">У меню " **керування** " виберіть пункт " **уніфіковане маркування**".</span><span class="sxs-lookup"><span data-stu-id="4334b-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="4334b-119">На **Лазуркому захист інформації – єдиний відповідний** клинок, натисніть кнопку **активувати** та дотримуйтеся вказівок в Інтернеті.</span><span class="sxs-lookup"><span data-stu-id="4334b-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="4334b-120">**Зверніть увагу**: переконайтеся, що у вас є відповідні дозволи, перш ніж активувати перенесення центру безпеки & відповідність.</span><span class="sxs-lookup"><span data-stu-id="4334b-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="4334b-121">Перегляньте ці статті, щоб отримати докладніші відомості.</span><span class="sxs-lookup"><span data-stu-id="4334b-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="4334b-122">Чи потрібно мати Глобальний адміністратор для налаштування захисту інформації в Azure, чи можна делегувати інших адміністраторів?</span><span class="sxs-lookup"><span data-stu-id="4334b-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="4334b-123">Важлива інформація про адміністративні ролі після переходу до центру відповідності безпеки &.</span><span class="sxs-lookup"><span data-stu-id="4334b-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="4334b-124">Щоб отримати докладніші відомості про службу "AIP" для об'єднаного маркування в центрі безпеки та відповідності, перегляньте статтю [перенесення етикеток](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="4334b-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
