---
title: Проблеми з використанням консолі адміністратора InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555882"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="b4932-102">Проблеми з використанням консолі адміністратора InTune</span><span class="sxs-lookup"><span data-stu-id="b4932-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="b4932-103">**"Немає доступу" під час переходу на портал адміністрування InTune.**</span><span class="sxs-lookup"><span data-stu-id="b4932-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="b4932-104">Якщо ви є членом настроюваної ролі InTune, переконайтеся, що для вашого облікового запису присвоюється ліцензія InTune або корпоративної мобільності (EMS).</span><span class="sxs-lookup"><span data-stu-id="b4932-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="b4932-105">Якщо використовується Диспетчер конфігурацій для керування пристроями, переконайтеся, що ви не є частиною колекції користувачів InTune для диспетчера конфігурацій MDM.</span><span class="sxs-lookup"><span data-stu-id="b4932-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="b4932-106">Переконайтеся, що вам призначено відповідні дозволи на основі ролей керування (RBAC), у "ролі InTune".</span><span class="sxs-lookup"><span data-stu-id="b4932-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="b4932-107">Перевірка групи, яка використовується, не є списком розсилки.</span><span class="sxs-lookup"><span data-stu-id="b4932-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="b4932-108">InTune на порталі Azure лише підтримує облікові записи користувачів, які належать до групи безпеки Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b4932-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="b4932-109">Перегляньте групи Azure порталу > **InTune**  >  **групи**або Azure портал > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="b4932-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="b4932-110">**Користувач має забагато дозволи на призначену роль InTune**</span><span class="sxs-lookup"><span data-stu-id="b4932-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="b4932-111">Консультування користувача, щоб перейти до **InTune**  >  **InTune ролей**  >  **мої дозволи**  >  на**експорт** , щоб переглянути надані дозволи.</span><span class="sxs-lookup"><span data-stu-id="b4932-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="b4932-112">**Я додав групу сфери до ролі, але користувачі в цій ролі все ще бачать інші користувачі або пристрої.**</span><span class="sxs-lookup"><span data-stu-id="b4932-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="b4932-113">Групи області не відфільтровувати користувачів або пристроїв.</span><span class="sxs-lookup"><span data-stu-id="b4932-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="b4932-114">Групи області:</span><span class="sxs-lookup"><span data-stu-id="b4932-114">Scope groups:</span></span>

- <span data-ttu-id="b4932-115">Обмеження, які користувачі можуть призначати політики або програми.</span><span class="sxs-lookup"><span data-stu-id="b4932-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="b4932-116">Дозволяти лише певним користувачам запускати віддалені завдання на пристроях.</span><span class="sxs-lookup"><span data-stu-id="b4932-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="b4932-117">Щоб отримати додаткові відомості про групи області, див [на основі ролей керування доступом (RBAC) з Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="b4932-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="b4932-118">**Я додав користувача до ролі InTune, але вони все ще мають повний доступ до консолі адміністратора InTune.**</span><span class="sxs-lookup"><span data-stu-id="b4932-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="b4932-119">Перейдіть до InTune > **користувачів** на порталі Azure і переконайтеся, що користувач не призначено для будь-якої з таких ролей на порталі Azure:</span><span class="sxs-lookup"><span data-stu-id="b4932-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="b4932-120">Глобальний адміністратор</span><span class="sxs-lookup"><span data-stu-id="b4932-120">Global administrator</span></span>
- <span data-ttu-id="b4932-121">InTune служби адміністратора</span><span class="sxs-lookup"><span data-stu-id="b4932-121">Intune service administrator</span></span>
- <span data-ttu-id="b4932-122">Адміністратор SharePoint</span><span class="sxs-lookup"><span data-stu-id="b4932-122">SharePoint administrator</span></span>

<span data-ttu-id="b4932-123">Для отримання додаткових відомостей зверніться [до служби керування доступом на основі ролей (RBAC) з Microsoft InTune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="b4932-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="b4932-124">**Проблеми з доступом**</span><span class="sxs-lookup"><span data-stu-id="b4932-124">**Access Issues**</span></span>

<span data-ttu-id="b4932-125">Щоб отримати додаткові відомості, [не вдається ввійти до Office 365, Azure або InTune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="b4932-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>