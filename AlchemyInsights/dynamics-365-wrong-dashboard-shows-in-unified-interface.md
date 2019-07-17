---
title: Dynamics 365 - неправильно Dashboard показує в єдиному інтерфейсі Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/16/2019
ms.locfileid: "35749109"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="959a7-102">Неправильно dashboard показує в єдиному інтерфейсі Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="959a7-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="959a7-103">Є кілька причин, чому ви можете побачити різні dashboard, ніж той, який ви очікуєте:</span><span class="sxs-lookup"><span data-stu-id="959a7-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="959a7-104">Користувач має встановити на приладній дошці користувача за промовчанням</span><span class="sxs-lookup"><span data-stu-id="959a7-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="959a7-105">Зазвичай можна ідентифікувати користувача за промовчанням dashboard встановити, якщо кнопку **Установити як значення за промовчанням** не відображається в панелі команд приладної дошки.</span><span class="sxs-lookup"><span data-stu-id="959a7-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="959a7-106">Приладна дошка користувача за промовчанням замінить усі інші за промовчанням приладні дошки, навіть якщо користувача за промовчанням приладної дошки не в поточному застосунку.</span><span class="sxs-lookup"><span data-stu-id="959a7-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="959a7-107">Використовуйте наступні обхідний шлях, щоб не використовувати їх за промовчанням dashboard.</span><span class="sxs-lookup"><span data-stu-id="959a7-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="959a7-108">Створення прикладної дошки, особистих.</span><span class="sxs-lookup"><span data-stu-id="959a7-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="959a7-109">Використовувати це Нова приладна дошка користувача за промовчанням.</span><span class="sxs-lookup"><span data-stu-id="959a7-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="959a7-110">Видалити цю приладну дошку.</span><span class="sxs-lookup"><span data-stu-id="959a7-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="959a7-111">Приладна дошка має значення у файлі sitemap</span><span class="sxs-lookup"><span data-stu-id="959a7-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="959a7-112">Встановлений в організації за промовчанням dashboard, вибравши приладної дошки та вибору "Встановити по замовчуванню" у розділі "Настройка системи".</span><span class="sxs-lookup"><span data-stu-id="959a7-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="959a7-113">Але dashboard, визначені в карта сайту дизайнер буде мати пріоритет над цієї приладної дошки, якщо користувач має доступ до нього.</span><span class="sxs-lookup"><span data-stu-id="959a7-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="959a7-114">Щоб користувачі побачити приладну дошку настроєно за промовчанням організації, ви можете:</span><span class="sxs-lookup"><span data-stu-id="959a7-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="959a7-115">Встановити цю приладну дошку в цьому файлі sitemap</span><span class="sxs-lookup"><span data-stu-id="959a7-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="959a7-116">Видалення доступу до приладної дошки sitemap, визначені для тих користувачів</span><span class="sxs-lookup"><span data-stu-id="959a7-116">Remove access to the sitemap defined dashboard for those users</span></span>
