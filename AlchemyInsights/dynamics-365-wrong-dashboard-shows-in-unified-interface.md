---
title: Приладна дошка Dynamics 365 – неправильна, у програмі Dynamics 365 уніфікований інтерфейс
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711296"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="fa1a7-102">Неправильна приладна дошка, що відображається в єдиному інтерфейсі Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="fa1a7-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="fa1a7-103">Існує кілька причин, через які можна побачити іншу приладну дошку, ніж очікувалося:</span><span class="sxs-lookup"><span data-stu-id="fa1a7-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="fa1a7-104">Користувач встановив приладну дошку користувача за замовчуванням</span><span class="sxs-lookup"><span data-stu-id="fa1a7-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="fa1a7-105">Зазвичай можна визначити приладну дошку користувача за замовчуванням, Якщо кнопка " **Установити за замовчуванням** " не відображається на панелі команд приладної дошки.</span><span class="sxs-lookup"><span data-stu-id="fa1a7-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="fa1a7-106">Приладна дошка користувача за замовчуванням замінить всі інші приладні дошки за замовчуванням, навіть якщо приладну дошку користувача за замовчуванням не відображається в поточній програмі.</span><span class="sxs-lookup"><span data-stu-id="fa1a7-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="fa1a7-107">Щоб не використовувати стандартну приладну дошку за замовчуванням, виконайте наведені нижче дії.</span><span class="sxs-lookup"><span data-stu-id="fa1a7-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="fa1a7-108">Створення нової персональної приладної дошки.</span><span class="sxs-lookup"><span data-stu-id="fa1a7-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="fa1a7-109">Установіть нову приладну дошку як користувача за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="fa1a7-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="fa1a7-110">Видаліть цю приладну дошку.</span><span class="sxs-lookup"><span data-stu-id="fa1a7-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="fa1a7-111">Приладна дошка встановлюється на карті сайту</span><span class="sxs-lookup"><span data-stu-id="fa1a7-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="fa1a7-112">Можливо, ви встановили приладну дошку організації за замовчуванням, вибравши приладну дошку та вибравши пункт "Установити за замовчуванням" в розділі "настроїти систему".</span><span class="sxs-lookup"><span data-stu-id="fa1a7-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="fa1a7-113">Але приладна дошка, визначена в конструкторі Sitemap, матиме пріоритет над цією приладною дошкою, якщо користувач має доступ до нього.</span><span class="sxs-lookup"><span data-stu-id="fa1a7-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="fa1a7-114">Щоб користувачі могли бачити приладну дошку, яку ви встановили як організацію за замовчуванням, можна виконати одну з таких дій:</span><span class="sxs-lookup"><span data-stu-id="fa1a7-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="fa1a7-115">Настроювання приладної дошки в карті сайту</span><span class="sxs-lookup"><span data-stu-id="fa1a7-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="fa1a7-116">Видалити доступ до визначеної приладної дошки Sitemap для цих користувачів</span><span class="sxs-lookup"><span data-stu-id="fa1a7-116">Remove access to the sitemap defined dashboard for those users</span></span>
