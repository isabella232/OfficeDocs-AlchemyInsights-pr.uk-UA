---
title: Обмежити SharePoint Online класичний режим
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 76f0b5ed67d3220559d25dfd72c7535181a4513b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761780"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="fa6a5-102">Обмежити SharePoint Online класичний режим</span><span class="sxs-lookup"><span data-stu-id="fa6a5-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="fa6a5-103">Деякі організації, як і раніше вимагають класичний режим досвід.</span><span class="sxs-lookup"><span data-stu-id="fa6a5-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="fa6a5-104">Хоча немає ніяких планів для видалення класичний режим рівні гранульований, це вже не можливо, щоб обмежити всієї організації (орендаря) класичний режим для списків і бібліотек.</span><span class="sxs-lookup"><span data-stu-id="fa6a5-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="fa6a5-105">Адміністратор буде мати такі параметри для керування окремими списками та бібліотеками в класичному режимі за допомогою гранульований відмовитися перемикачі, які ми надаємо на наступних рівнях:</span><span class="sxs-lookup"><span data-stu-id="fa6a5-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="fa6a5-106">колекції сайтів</span><span class="sxs-lookup"><span data-stu-id="fa6a5-106">site collection</span></span>
- <span data-ttu-id="fa6a5-107">сайт</span><span class="sxs-lookup"><span data-stu-id="fa6a5-107">site</span></span>
- <span data-ttu-id="fa6a5-108">Список</span><span class="sxs-lookup"><span data-stu-id="fa6a5-108">list</span></span>
- <span data-ttu-id="fa6a5-109">Бібліотека</span><span class="sxs-lookup"><span data-stu-id="fa6a5-109">library</span></span>

<span data-ttu-id="fa6a5-110">Крім того, списки, що використання деяких функцій і настройок, які не підтримуються сучасного буде ще бути автоматично перемикається в класичному режимі.</span><span class="sxs-lookup"><span data-stu-id="fa6a5-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="fa6a5-111">Починаючи з 1 квітня 2019, процес вимкнення орендар рівень відмовитися від сучасних список і бібліотек почати і продовжити через 31 травня 2019.</span><span class="sxs-lookup"><span data-stu-id="fa6a5-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="fa6a5-112">Списків і бібліотек, які знаходяться в класичному режимі в результаті орендар відмовитися буде автоматично зміщуватися до сучасних.</span><span class="sxs-lookup"><span data-stu-id="fa6a5-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="fa6a5-113">Якщо вам потрібна класичний режим будь ласка Докладніше [тут](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) і PnP Powershell інструкція [тут](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , описаній опцій і інструментів, які можна використовувати сьогодні, щоб використовувати класичний режим досвід.</span><span class="sxs-lookup"><span data-stu-id="fa6a5-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
