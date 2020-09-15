---
title: Заміна вашого класичного кореневого сайту на сучасний сайт
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691200"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="cfae6-102">Заміна вашого класичного кореневого сайту на сучасний сайт</span><span class="sxs-lookup"><span data-stu-id="cfae6-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="cfae6-103">Якщо ваше середовище настроєно до квітня 2019, ви можете змінити кореневий сайт на сучасний сайт за допомогою Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="cfae6-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="cfae6-104">Якщо у вас інший сайт, який потрібно використовувати як кореневий сайт, можна замінити [(своп) кореневим сайтом](https://docs.microsoft.com/sharepoint/modern-root-site) .</span><span class="sxs-lookup"><span data-stu-id="cfae6-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="cfae6-105">Використовуйте функцію [виклику-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , щоб поміняти місцями розташування сайту з іншим сайтом під час архівації оригінального сайту.</span><span class="sxs-lookup"><span data-stu-id="cfae6-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="cfae6-106">Доступно для сайту групи (не підключено до групи) і сайту зв'язку.</span><span class="sxs-lookup"><span data-stu-id="cfae6-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="cfae6-107">Незабаром буде запропоновано додаткові можливості, які дозволять вам надалі використовувати вміст на сайті, але перетворити наявний сайт на сайт спілкування.</span><span class="sxs-lookup"><span data-stu-id="cfae6-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="cfae6-108">Ці можливості буде розгорнуто поступово.</span><span class="sxs-lookup"><span data-stu-id="cfae6-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="cfae6-109">Продовжуйте перевіряти центр повідомлень для оновлень.</span><span class="sxs-lookup"><span data-stu-id="cfae6-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="cfae6-110">Відомі проблеми з відповідними сайтами</span><span class="sxs-lookup"><span data-stu-id="cfae6-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="cfae6-111">Цільовий сайт може повернути помилку "не знайдено" (HTTP 404) за короткий проміжок часу.</span><span class="sxs-lookup"><span data-stu-id="cfae6-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="cfae6-112">Вміст має бути переведена для оновлення індексу пошуку.</span><span class="sxs-lookup"><span data-stu-id="cfae6-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="cfae6-113">Не потрібно виконувати ручний крок – це буде здійснюватися автоматично.</span><span class="sxs-lookup"><span data-stu-id="cfae6-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="cfae6-114">Все, що залежить від "статичних" посилань (наприклад, синхронізації файлів і файлів OneNote), потрібно буде виправити вручну.</span><span class="sxs-lookup"><span data-stu-id="cfae6-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="cfae6-115">Якщо вихідний сайт став організаційним сайтом новин, оновіть URL-адресу.</span><span class="sxs-lookup"><span data-stu-id="cfae6-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="cfae6-116">Отримайте список усіх організаційних сайтів новин.</span><span class="sxs-lookup"><span data-stu-id="cfae6-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="cfae6-117">Сайти Project Server, можливо, потрібно перевірити, щоб переконатися, що вони все ще пов'язані належним чином.</span><span class="sxs-lookup"><span data-stu-id="cfae6-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
