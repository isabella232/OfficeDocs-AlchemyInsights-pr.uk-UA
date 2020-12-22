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
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724175"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="9d5b7-102">Примітки з елементами списку</span><span class="sxs-lookup"><span data-stu-id="9d5b7-102">Comments on List items</span></span>

<span data-ttu-id="9d5b7-103">Користувачі можуть переглядати всі примітки в елементі списку та фільтрувати подання, які показують примітки або дії, пов'язані з елементом.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="9d5b7-104">Щоб додати та видалити примітки, потрібно звернути увагу на такі користувачі:</span><span class="sxs-lookup"><span data-stu-id="9d5b7-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="9d5b7-105">Примітки, які відповідають параметрам дозволів, притаманних службі SharePoint.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="9d5b7-106">Класичні списки, які ще не вбудовані для відображення в сучасних інтерфейсах користувача, як-от списки завдань, не можуть мати цю функцію коментування.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="9d5b7-107">У цьому випуску не можна коментувати списки в командах.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="9d5b7-108">Примітки не індексуються за допомогою функції пошуку.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="9d5b7-109">Адміністратори можуть вимкнути цю функцію на рівні організації, змінивши параметр **Commitsonlistitemplesвідключені** у командлет **Set-spotenant** PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="9d5b7-110">Зараз не можна вимкнути коментування на веб-сайті або рівні списку.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="9d5b7-111">Ми сподіваємося, що ці елементи керування в подальшому оновленні, ймовірно, у першому кварталі 2021.</span><span class="sxs-lookup"><span data-stu-id="9d5b7-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
