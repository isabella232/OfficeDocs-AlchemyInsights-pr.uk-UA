---
title: Сучасний сайт як корінь сайту
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543874"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="323f2-102">Сучасний сайт як корінь сайту</span><span class="sxs-lookup"><span data-stu-id="323f2-102">Modern site as root site</span></span>

<span data-ttu-id="323f2-103">Ми почали свиті нова функція, яка дозволить вам swap свій класичний сайт кореневий сайт з сучасними сайту.</span><span class="sxs-lookup"><span data-stu-id="323f2-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="323f2-104">Міняти місцями розташування сайт з іншого сайту час архівації на оригінальний сайт за допомогою [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="323f2-104">Use [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="323f2-105">Доступні для сайту групи (не підключено до групи) і повідомлення сайту.</span><span class="sxs-lookup"><span data-stu-id="323f2-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="323f2-106">Не видалити ваш класичний кореневий сайт для створення сучасного повідомлення сайту.</span><span class="sxs-lookup"><span data-stu-id="323f2-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="323f2-107">Це не підтримується корпорацією Майкрософт.</span><span class="sxs-lookup"><span data-stu-id="323f2-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="323f2-108">Видалення кореневий сайт буде зробити всі сайти SharePoint у вашій організації недоступними для всіх користувачів, доки ви не відновити сайту або створіть новий сайт в той же URL.</span><span class="sxs-lookup"><span data-stu-id="323f2-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="323f2-109">Ми будемо спілкуватися цю функцію через центр повідомлення.</span><span class="sxs-lookup"><span data-stu-id="323f2-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="323f2-110">Ви повинні чекати, цю функцію можна ввімкнути у вашому орендар незабаром.</span><span class="sxs-lookup"><span data-stu-id="323f2-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="323f2-111">Відомих проблем із заміни сайти</span><span class="sxs-lookup"><span data-stu-id="323f2-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="323f2-112">Цільовий сайт може повернути "не знайдено" помилка (HTTP 404) протягом короткого періоду часу.</span><span class="sxs-lookup"><span data-stu-id="323f2-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="323f2-113">Вміст потрібно буде виконано оновлення індексу пошуку.</span><span class="sxs-lookup"><span data-stu-id="323f2-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="323f2-114">Немає не ручного кроку потрібно тут, це буде зроблено автоматично.</span><span class="sxs-lookup"><span data-stu-id="323f2-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="323f2-115">Все, що залежить від "статичний" посилання (наприклад синхронізації файлів і OneNote файли) потрібно буде вручну виправити.</span><span class="sxs-lookup"><span data-stu-id="323f2-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="323f2-116">Project Server сайтів, можливо, доведеться можна перевірити, щоб переконатися, що вони, як і раніше пов'язані правильно.</span><span class="sxs-lookup"><span data-stu-id="323f2-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
