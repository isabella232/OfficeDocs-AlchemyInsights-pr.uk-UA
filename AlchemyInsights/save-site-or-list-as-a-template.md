---
title: Зберегти сайт або список як шаблон
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048745"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="3fd42-102">Зберегти сайт або список як шаблон</span><span class="sxs-lookup"><span data-stu-id="3fd42-102">Save site or list as a template</span></span>

<span data-ttu-id="3fd42-103">Шаблони сайтів SharePoint – це заздалегідь створені визначення, створені навколо певної бізнес-потреби.</span><span class="sxs-lookup"><span data-stu-id="3fd42-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="3fd42-104">Для отримання додаткових відомостей див. [використання шаблонів для створення різних типів сайтів SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="3fd42-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="3fd42-105">Нижче наведено деякі поширені проблеми/рішення щодо збереження сайту або списку як шаблону в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="3fd42-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="3fd42-106">**Зберегти сайт/шаблон списку кнопка недоступна або відсутня**.</span><span class="sxs-lookup"><span data-stu-id="3fd42-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="3fd42-107">Адміністраторам потрібно буде дозволити користувацький скрипт для ввімкнення функцій шаблону.</span><span class="sxs-lookup"><span data-stu-id="3fd42-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="3fd42-108">Докладні кроки, приклади та [міркування див.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)</span><span class="sxs-lookup"><span data-stu-id="3fd42-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="3fd42-109">Команда Зберегти як шаблон не підтримується і може спричинити проблеми на веб-сайтах, які використовують видавничу інфраструктуру SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="3fd42-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="3fd42-110">**Не вдалося створити шаблон сайту або не працює належним чином**</span><span class="sxs-lookup"><span data-stu-id="3fd42-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="3fd42-111">Можливо, шаблон відсутній, а [функція](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) не активується.</span><span class="sxs-lookup"><span data-stu-id="3fd42-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="3fd42-112">Якщо функція недоступна для активації в поточній колекції сайтів, не можна використовувати шаблон сайту для створення сайту.</span><span class="sxs-lookup"><span data-stu-id="3fd42-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="3fd42-113">Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 елементів, оскільки це може блокувати створення шаблону сайту.</span><span class="sxs-lookup"><span data-stu-id="3fd42-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="3fd42-114">Можливо, сайт використовує забагато ресурсів, і тому шаблон сайту перевищує ліміт 50 мегабайт (МБ).</span><span class="sxs-lookup"><span data-stu-id="3fd42-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="3fd42-115">Є проблеми з відображенням даних зі списку, який використовує стовпець підстановки.</span><span class="sxs-lookup"><span data-stu-id="3fd42-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="3fd42-116">Для отримання додаткових відомостей див. у [списку шаблон не відображаються дані зі списку правильні підстановки в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="3fd42-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="3fd42-117">Для отримання більш детальної інформації про загальні проблеми та рішення, будь ласка, посилання, [створювати і використовувати шаблони сайту](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="3fd42-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

