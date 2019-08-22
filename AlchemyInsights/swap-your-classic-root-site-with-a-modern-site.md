---
title: Swap свій класичний кореневий сайт з сучасними сайту
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: ffb1466fe436d6cab7ae5fdd60c671f5dd2654dd
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36501100"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="b01bb-102">Swap свій класичний кореневий сайт з сучасними сайту</span><span class="sxs-lookup"><span data-stu-id="b01bb-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="b01bb-103">Ваше оточення було створено раніше квітня 2019, змініть кореневий сайт на сучасний сайт за допомогою Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="b01bb-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="b01bb-104">Якщо у вас є інший сайт, який ви бажаєте використовувати як корінь сайту, можна замінити (свопу) кореневий сайт його.</span><span class="sxs-lookup"><span data-stu-id="b01bb-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="b01bb-105">Міняти місцями розташування сайт з іншого сайту час архівації на оригінальний сайт за допомогою [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="b01bb-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="b01bb-106">Доступні для сайту групи (не підключено до групи) і повідомлення сайту.</span><span class="sxs-lookup"><span data-stu-id="b01bb-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="b01bb-107">Додаткові можливості будуть введені незабаром що дасть змогу продовжувати використовувати вміст на сайті, але перетворити наявний сайт повідомлення сайту.</span><span class="sxs-lookup"><span data-stu-id="b01bb-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="b01bb-108">Ці можливості буде поширена поступово.</span><span class="sxs-lookup"><span data-stu-id="b01bb-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="b01bb-109">Як і раніше перевірити Office 365 повідомлення центр оновлень.</span><span class="sxs-lookup"><span data-stu-id="b01bb-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="b01bb-110">Відомих проблем із заміни сайти</span><span class="sxs-lookup"><span data-stu-id="b01bb-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="b01bb-111">Цільовий сайт може повернути "не знайдено" помилка (HTTP 404) протягом короткого періоду часу.</span><span class="sxs-lookup"><span data-stu-id="b01bb-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="b01bb-112">Вміст потрібно буде виконано оновлення індексу пошуку.</span><span class="sxs-lookup"><span data-stu-id="b01bb-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="b01bb-113">Немає не ручного кроку потрібно - це буде зроблено автоматично.</span><span class="sxs-lookup"><span data-stu-id="b01bb-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="b01bb-114">Все, що залежить від "статичний" посилання (наприклад синхронізації файлів і OneNote файли) потрібно буде вручну виправити.</span><span class="sxs-lookup"><span data-stu-id="b01bb-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="b01bb-115">Якщо вихідний сайт був організаційні новини сайту, оновлення URL.</span><span class="sxs-lookup"><span data-stu-id="b01bb-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="b01bb-116">Отримати список всіх організаційних новинні сайти.</span><span class="sxs-lookup"><span data-stu-id="b01bb-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="b01bb-117">Project Server сайтів, можливо, доведеться можна перевірити, щоб переконатися, що вони, як і раніше пов'язані правильно.</span><span class="sxs-lookup"><span data-stu-id="b01bb-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





