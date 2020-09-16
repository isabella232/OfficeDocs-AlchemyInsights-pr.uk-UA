---
title: Збереження сайту або списку як шаблону
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727552"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="91239-102">Збереження сайту або списку як шаблону</span><span class="sxs-lookup"><span data-stu-id="91239-102">Save site or list as a template</span></span>

<span data-ttu-id="91239-103">Шаблони сайтів SharePoint – це попередньо створені визначення, розроблені навколо певної потреби бізнесу.</span><span class="sxs-lookup"><span data-stu-id="91239-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="91239-104">Докладні відомості наведено в статті [використання шаблонів для створення різних типів сайтів SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="91239-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="91239-105">Нижче наведено кілька поширених проблем і рішень щодо збереження сайту або списку як шаблону в службі SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="91239-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="91239-106">**Кнопка збереження шаблону сайту або списку недоступна або відсутня**.</span><span class="sxs-lookup"><span data-stu-id="91239-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="91239-107">Адміністраторам потрібно дозволити настроюваний сценарій для ввімкнення функцій шаблону.</span><span class="sxs-lookup"><span data-stu-id="91239-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="91239-108">Докладні вказівки, приклади та міркування [дають змогу переглянути або заборонити настроюваний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="91239-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="91239-109">Команда "зберегти сайт як шаблон" не підтримується та може спричинити проблеми на сайтах, які використовують інфраструктуру публікування SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="91239-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="91239-110">**Не вдалося створити шаблон сайту або не працює належним чином**</span><span class="sxs-lookup"><span data-stu-id="91239-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="91239-111">Можливо, у шаблоні немає [функції](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , і його не активовано.</span><span class="sxs-lookup"><span data-stu-id="91239-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="91239-112">Якщо функція недоступна для активації в поточній колекції сайтів, шаблон сайту не можна використовувати для створення сайту.</span><span class="sxs-lookup"><span data-stu-id="91239-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="91239-113">Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) в пунктах 5000, оскільки це може заблокувати створення шаблону сайту.</span><span class="sxs-lookup"><span data-stu-id="91239-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="91239-114">Сайт може використовувати забагато ресурсів, тому шаблон сайту перевищує обмеження 50 мегабайт (МБ).</span><span class="sxs-lookup"><span data-stu-id="91239-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="91239-115">Під час відображення даних зі списку, у якому використовується стовпець підстановки, виникають проблеми.</span><span class="sxs-lookup"><span data-stu-id="91239-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="91239-116">Щоб отримати докладніші відомості, [у списку в службі SharePoint Online не відображаються дані зі списку правильних підстановок](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="91239-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="91239-117">Щоб отримати докладні відомості про поширені проблеми та рішення, Дізнайтеся, як [створювати та використовувати шаблони сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="91239-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

