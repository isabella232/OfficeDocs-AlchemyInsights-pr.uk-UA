---
title: Примітки з елементами списку
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982553"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="6583e-102">Примітки з елементами списку</span><span class="sxs-lookup"><span data-stu-id="6583e-102">Comments on List items</span></span>

<span data-ttu-id="6583e-103">Користувачі зможуть незабаром додавати та видаляти примітки в елементах списку.</span><span class="sxs-lookup"><span data-stu-id="6583e-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="6583e-104">Користувачі можуть переглядати всі примітки в елементі списку та фільтрувати подання, які показують примітки або дії, пов'язані з елементом.</span><span class="sxs-lookup"><span data-stu-id="6583e-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="6583e-105">**Хронометраж** :</span><span class="sxs-lookup"><span data-stu-id="6583e-105">**Timing** :</span></span>

<span data-ttu-id="6583e-106">**Цільовий випуск** : поступове взяття на редагування в середині жовтня і очікується завершення до середини листопада</span><span class="sxs-lookup"><span data-stu-id="6583e-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="6583e-107">**Стандартний випуск** : поступове вивідати в середині листопада і очікується завершення на початок грудня</span><span class="sxs-lookup"><span data-stu-id="6583e-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="6583e-108">**Впровадження** : цільовий випуск для всієї організації</span><span class="sxs-lookup"><span data-stu-id="6583e-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="6583e-109">Щоб додати та видалити примітки, потрібно звернути увагу на такі користувачі:</span><span class="sxs-lookup"><span data-stu-id="6583e-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="6583e-110">Примітки, які відповідають параметрам дозволів, притаманних службі SharePoint.</span><span class="sxs-lookup"><span data-stu-id="6583e-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="6583e-111">Класичні списки, які ще не вбудовані для відображення в сучасних інтерфейсах користувача, як-от списки завдань, не можуть мати цю функцію коментування.</span><span class="sxs-lookup"><span data-stu-id="6583e-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="6583e-112">У цьому випуску не можна коментувати списки в командах.</span><span class="sxs-lookup"><span data-stu-id="6583e-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="6583e-113">Примітки не індексуються за допомогою функції пошуку.</span><span class="sxs-lookup"><span data-stu-id="6583e-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="6583e-114">Адміністратори можуть вимкнути цю функцію на рівні організації, змінивши параметр **Commitsonlistitemplesвідключені** у командлет **Set-spotenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6583e-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="6583e-115">Зараз не можна вимкнути коментування на веб-сайті або рівні списку.</span><span class="sxs-lookup"><span data-stu-id="6583e-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="6583e-116">Ми сподіваємося, що ці елементи керування в подальшому оновленні, ймовірно, у першому кварталі 2021.</span><span class="sxs-lookup"><span data-stu-id="6583e-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
