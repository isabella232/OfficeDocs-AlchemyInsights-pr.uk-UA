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
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: e7ecfd8c2f1a532355bfb8c2c0a846fc0d6e88b1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551580"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="3ac94-102">Обмежити SharePoint Online класичний режим</span><span class="sxs-lookup"><span data-stu-id="3ac94-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="3ac94-103">Деякі організації, як і раніше вимагають класичний режим досвід.</span><span class="sxs-lookup"><span data-stu-id="3ac94-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="3ac94-104">Хоча немає ніяких планів для видалення класичний режим рівні гранульований, це вже не можливо, щоб обмежити всієї організації (орендаря) класичний режим для списків і бібліотек.</span><span class="sxs-lookup"><span data-stu-id="3ac94-104">While there are no plans to remove classic mode at a granular level, it is no longer possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="3ac94-105">Адміністратор буде мати такі параметри для керування окремими списками та бібліотеками в класичному режимі за допомогою гранульований відмовитися перемикачі, які ми надаємо на наступних рівнях:</span><span class="sxs-lookup"><span data-stu-id="3ac94-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

- <span data-ttu-id="3ac94-106">колекції сайтів</span><span class="sxs-lookup"><span data-stu-id="3ac94-106">site collection</span></span>
- <span data-ttu-id="3ac94-107">сайт</span><span class="sxs-lookup"><span data-stu-id="3ac94-107">site</span></span>
- <span data-ttu-id="3ac94-108">Список</span><span class="sxs-lookup"><span data-stu-id="3ac94-108">list</span></span>
- <span data-ttu-id="3ac94-109">Бібліотека</span><span class="sxs-lookup"><span data-stu-id="3ac94-109">library</span></span>

<span data-ttu-id="3ac94-110">Крім того, списки, що використання деяких функцій і настройок, які не підтримуються сучасного буде ще бути автоматично перемикається в класичному режимі.</span><span class="sxs-lookup"><span data-stu-id="3ac94-110">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="3ac94-111">Починаючи з 1 квітня 2019, процес вимкнення орендар рівень відмовитися від сучасних список і бібліотек почати і продовжити через 31 травня 2019.</span><span class="sxs-lookup"><span data-stu-id="3ac94-111">Beginning April 1, 2019, the process to disable the tenant level opt out of modern list and libraries will start and continue through May 31, 2019.</span></span>  <span data-ttu-id="3ac94-112">Списків і бібліотек, які знаходяться в класичному режимі в результаті орендар відмовитися буде автоматично зміщуватися до сучасних.</span><span class="sxs-lookup"><span data-stu-id="3ac94-112">The lists and libraries that are in classic mode as a result of tenant opt-out will automatically be shifted to modern.</span></span>

<span data-ttu-id="3ac94-113">Якщо вам потрібна класичний режим будь ласка Докладніше [тут](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) і PnP Powershell інструкція [тут](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) , описаній опцій і інструментів, які можна використовувати сьогодні, щоб використовувати класичний режим досвід.</span><span class="sxs-lookup"><span data-stu-id="3ac94-113">If you require classic mode please see more information [here](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) and PnP Powershell instruction [here](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) that describes options and tools you can use today to use the classic mode experience.</span></span>
