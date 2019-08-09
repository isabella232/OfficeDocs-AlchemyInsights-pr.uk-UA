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
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270765"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="ea3b5-102">Swap свій класичний кореневий сайт з сучасними сайту</span><span class="sxs-lookup"><span data-stu-id="ea3b5-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="ea3b5-103">Ваше оточення було створено раніше квітня 2019, змініть кореневий сайт на сучасний сайт за допомогою Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ea3b5-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="ea3b5-104">Якщо у вас є інший сайт, який ви бажаєте використовувати як корінь сайту, можна замінити (свопу) кореневий сайт його.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-104">If you have a different site that you want to use as your root site, you can replace (swap) the root site with it.</span></span> 
    - <span data-ttu-id="ea3b5-105">Міняти місцями розташування сайт з іншого сайту час архівації на оригінальний сайт за допомогою [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="ea3b5-105">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="ea3b5-106">Доступні для сайту групи (не підключено до групи) і повідомлення сайту.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="ea3b5-107">Додаткові можливості будуть введені незабаром що дасть змогу продовжувати використовувати вміст на сайті, але перетворити наявний сайт повідомлення сайту.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="ea3b5-108">Ці можливості буде поширена поступово.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="ea3b5-109">Як і раніше перевірити Office 365 повідомлення центр оновлень.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-109">Continue to check the Office 365 Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="ea3b5-110">Відомих проблем із заміни сайти</span><span class="sxs-lookup"><span data-stu-id="ea3b5-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="ea3b5-111">Цільовий сайт може повернути "не знайдено" помилка (HTTP 404) протягом короткого періоду часу.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="ea3b5-112">Вміст потрібно буде виконано оновлення індексу пошуку.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="ea3b5-113">Немає не ручного кроку потрібно - це буде зроблено автоматично.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="ea3b5-114">Все, що залежить від "статичний" посилання (наприклад синхронізації файлів і OneNote файли) потрібно буде вручну виправити.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="ea3b5-115">Якщо вихідний сайт був організаційні новини сайту, оновлення URL.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="ea3b5-116">Отримати список всіх організаційних новинні сайти.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="ea3b5-117">Project Server сайтів, можливо, доведеться можна перевірити, щоб переконатися, що вони, як і раніше пов'язані правильно.</span><span class="sxs-lookup"><span data-stu-id="ea3b5-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>





