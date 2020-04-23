---
title: Своп ваш класичний кореневий сайт з сучасним сайтом
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741565"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="9a7d8-102">Своп ваш класичний кореневий сайт з сучасним сайтом</span><span class="sxs-lookup"><span data-stu-id="9a7d8-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="9a7d8-103">Якщо ваше оточення було настроєно до квітня 2019, ви можете змінити свій кореневий сайт на сучасний сайт за допомогою Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="9a7d8-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="9a7d8-104">Якщо у вас є інший сайт, який ви хочете використовувати як ваш кореневий сайт, ви можете замінити [(Swap) кореневий сайт](https://docs.microsoft.com/sharepoint/modern-root-site) з ним.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="9a7d8-105">Використовуйте [виклик-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , щоб поміняти місцями розташування сайту на інший сайт під час архівування оригінального сайту.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="9a7d8-106">Доступно як для команди сайту (не підключеної до групи), так і на сайті зв'язку.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="9a7d8-107">Додаткові можливості будуть введені найближчим часом, що дозволить вам продовжувати використовувати контент на сайті, але перетворити існуючий сайт на сайт зв'язку.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="9a7d8-108">Ці можливості будуть розгорнута поступово.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="9a7d8-109">Продовжуйте перевіряти наявність оновлень у центрі повідомлень.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="9a7d8-110">Відомі проблеми з місцями для заміни</span><span class="sxs-lookup"><span data-stu-id="9a7d8-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="9a7d8-111">Цільовий сайт може повернути помилка "не знайдено" (HTTP 404) протягом короткого періоду часу.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="9a7d8-112">Для оновлення індексу пошуку потрібно буде оновити вміст.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="9a7d8-113">Немає потрібного кроку вручну-це буде зроблено автоматично.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="9a7d8-114">Все залежить від "статичних" посилань (наприклад, синхронізації файлів і файлів OneNote) потрібно буде вручну виправити.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="9a7d8-115">Якщо вихідний сайт був організаційним сайтом новин, оновіть URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="9a7d8-116">Отримайте список всіх організаційних новинних сайтів.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="9a7d8-117">Сайти Project Server, можливо, потрібно перевірити, щоб переконатися, що вони все ще пов'язані належним чином.</span><span class="sxs-lookup"><span data-stu-id="9a7d8-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
