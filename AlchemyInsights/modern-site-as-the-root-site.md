---
title: Сучасний сайт як кореневий сайт
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713812"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="97d9c-102">Сучасний сайт як кореневий сайт</span><span class="sxs-lookup"><span data-stu-id="97d9c-102">Modern site as root site</span></span>

<span data-ttu-id="97d9c-103">Ми почали розгортання нової функції, яка дозволить вам [поміняти ваш класичний сайт кореневого сайту з сучасним сайтом](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="97d9c-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="97d9c-104">Використовуйте [виклик-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , щоб поміняти місцями розташування сайту на інший сайт під час архівування оригінального сайту.</span><span class="sxs-lookup"><span data-stu-id="97d9c-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="97d9c-105">Доступно як для команди сайту (не підключеної до групи), так і на сайті зв'язку.</span><span class="sxs-lookup"><span data-stu-id="97d9c-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="97d9c-106">Не видаляйте свій класичний кореневий сайт, щоб створити сучасний сайт для спілкування.</span><span class="sxs-lookup"><span data-stu-id="97d9c-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="97d9c-107">Це не підтримується Microsoft.</span><span class="sxs-lookup"><span data-stu-id="97d9c-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="97d9c-108">Видалення кореневого сайту призведе до того, що всі сайти SharePoint у вашій організації недоступні для всіх користувачів, доки ви не відновите сайт або не створите новий сайт за такою ж URL-адресою.</span><span class="sxs-lookup"><span data-stu-id="97d9c-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="97d9c-109">Ми будемо спілкуватися цю функцію через центр повідомлень.</span><span class="sxs-lookup"><span data-stu-id="97d9c-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="97d9c-110">Ви повинні очікувати, що функція повинна бути включена в ваш орендар найближчим часом.</span><span class="sxs-lookup"><span data-stu-id="97d9c-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="97d9c-111">Відомі проблеми з місцями для заміни</span><span class="sxs-lookup"><span data-stu-id="97d9c-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="97d9c-112">Цільовий сайт може повернути помилка "не знайдено" (HTTP 404) протягом короткого періоду часу.</span><span class="sxs-lookup"><span data-stu-id="97d9c-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="97d9c-113">Для оновлення індексу пошуку потрібно буде оновити вміст.</span><span class="sxs-lookup"><span data-stu-id="97d9c-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="97d9c-114">Тут немає потрібного кроку вручну, це буде зроблено автоматично.</span><span class="sxs-lookup"><span data-stu-id="97d9c-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="97d9c-115">Все залежить від "статичних" посилань (наприклад, синхронізації файлів і файлів OneNote) потрібно буде вручну виправити.</span><span class="sxs-lookup"><span data-stu-id="97d9c-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="97d9c-116">Сайти Project Server, можливо, потрібно перевірити, щоб переконатися, що вони все ще пов'язані належним чином.</span><span class="sxs-lookup"><span data-stu-id="97d9c-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
