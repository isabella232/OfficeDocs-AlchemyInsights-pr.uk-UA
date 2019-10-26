---
title: Dynamics 365-неправильна приладна дошка відображається в Dynamics 365 єдиному інтерфейсі
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36528572"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="6249a-102">Неправильна приладна дошка показує в Dynamics 365 єдиному інтерфейсі</span><span class="sxs-lookup"><span data-stu-id="6249a-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="6249a-103">Існує кілька причин, чому ви можете побачити іншу приладну дошку, ніж очікувалося:</span><span class="sxs-lookup"><span data-stu-id="6249a-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="6249a-104">Користувач встановити приладну дошку користувача за промовчанням</span><span class="sxs-lookup"><span data-stu-id="6249a-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="6249a-105">Зазвичай ви можете визначити користувацьку приладну дошку за промовчанням, Якщо кнопка **Установити як за промовчанням** не відображається на панелі команд приладної дошки.</span><span class="sxs-lookup"><span data-stu-id="6249a-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="6249a-106">Приладна дошка користувача за промовчанням замінить всі інші приладні дошки за промовчанням, навіть якщо приладна дошка за промовчанням користувача не перебуває в поточній програмі.</span><span class="sxs-lookup"><span data-stu-id="6249a-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="6249a-107">Скористайтеся таким обхідним шляхом, щоб не використовувати приладну дошку за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="6249a-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="6249a-108">Створити нову особисту приладну дошку.</span><span class="sxs-lookup"><span data-stu-id="6249a-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="6249a-109">Встановіть нову приладну дошку як користувацьку за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="6249a-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="6249a-110">Видалити цю приладну дошку.</span><span class="sxs-lookup"><span data-stu-id="6249a-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="6249a-111">Приладна дошка встановлюється на карті сайту</span><span class="sxs-lookup"><span data-stu-id="6249a-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="6249a-112">Можливо, ви встановили приладну дошку організації за замовчуванням, вибравши приладну дошку та вибравши "встановити за умовчанням" у розділі "налаштувати систему".</span><span class="sxs-lookup"><span data-stu-id="6249a-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="6249a-113">Але приладна дошка, визначена в конструкторі Sitemap, буде мати пріоритет над цією панеллю, якщо користувач має доступ до нього.</span><span class="sxs-lookup"><span data-stu-id="6249a-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="6249a-114">Щоб користувачі бачили приладну дошку, яку ви встановили як організацію за замовчуванням, ви можете або:</span><span class="sxs-lookup"><span data-stu-id="6249a-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="6249a-115">Установити цю приладну дошку на карті сайту</span><span class="sxs-lookup"><span data-stu-id="6249a-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="6249a-116">Скасуйте доступ до визначеної приладної дошки сайту для цих користувачів</span><span class="sxs-lookup"><span data-stu-id="6249a-116">Remove access to the sitemap defined dashboard for those users</span></span>
