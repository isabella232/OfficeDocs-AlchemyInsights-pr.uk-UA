---
title: Сучасний сайт як кореневий сайт
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666891"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="df91f-102">Сучасний сайт як кореневий сайт</span><span class="sxs-lookup"><span data-stu-id="df91f-102">Modern site as root site</span></span>

<span data-ttu-id="df91f-103">Ми почали використовувати нову функцію, яка дозволить вам [обміняти ваш класичний сайт кореневого сайту на сучасний сайт](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="df91f-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="df91f-104">Використовуйте функцію [виклику-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) , щоб поміняти місцями розташування сайту з іншим сайтом під час архівації оригінального сайту.</span><span class="sxs-lookup"><span data-stu-id="df91f-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="df91f-105">Доступно для сайту групи (не підключено до групи) і сайту зв'язку.</span><span class="sxs-lookup"><span data-stu-id="df91f-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="df91f-106">Не видаляйте свій класичний кореневий сайт, щоб створити сучасний сайт для спілкування.</span><span class="sxs-lookup"><span data-stu-id="df91f-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="df91f-107">Корпорація Майкрософт не підтримує цю підтримку.</span><span class="sxs-lookup"><span data-stu-id="df91f-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="df91f-108">Якщо видалити кореневий сайт, усі сайти SharePoint у вашій організації недоступні для всіх користувачів, доки ви не відновлюєте сайт або не створюєте новий сайт з тієї самої URL-адресою.</span><span class="sxs-lookup"><span data-stu-id="df91f-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="df91f-109">Ми будемо спілкуватися з цією функцією через центр повідомлень.</span><span class="sxs-lookup"><span data-stu-id="df91f-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="df91f-110">Ви маєте очікувати, що функція має активуватися в клієнті найближчим часом.</span><span class="sxs-lookup"><span data-stu-id="df91f-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="df91f-111">Відомі проблеми з відповідними сайтами</span><span class="sxs-lookup"><span data-stu-id="df91f-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="df91f-112">Цільовий сайт може повернути помилку "не знайдено" (HTTP 404) за короткий проміжок часу.</span><span class="sxs-lookup"><span data-stu-id="df91f-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="df91f-113">Вміст має бути переведена для оновлення індексу пошуку.</span><span class="sxs-lookup"><span data-stu-id="df91f-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="df91f-114">Для цього не потрібно виконати ручний крок, це буде здійснюватися автоматично.</span><span class="sxs-lookup"><span data-stu-id="df91f-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="df91f-115">Все, що залежить від "статичних" посилань (наприклад, синхронізації файлів і файлів OneNote), потрібно буде виправити вручну.</span><span class="sxs-lookup"><span data-stu-id="df91f-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="df91f-116">Сайти Project Server, можливо, потрібно перевірити, щоб переконатися, що вони все ще пов'язані належним чином.</span><span class="sxs-lookup"><span data-stu-id="df91f-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
