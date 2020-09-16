---
title: Створення сайту в службі SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732266"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="57d6d-102">Створення сайтів SharePoint за допомогою шаблонів</span><span class="sxs-lookup"><span data-stu-id="57d6d-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="57d6d-103">Можливість зберегти сайт як шаблон не підтримується на сучасних сайтах спілкування або груп.</span><span class="sxs-lookup"><span data-stu-id="57d6d-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="57d6d-104">Докладні відомості про використання шаблонів наведено в статті [збереження, завантаження та передавання сайту SharePoint як шаблону](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="57d6d-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="57d6d-105">Нижче наведено кілька поширених проблем і рішень щодо збереження сайту або списку як шаблону в службі SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="57d6d-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="57d6d-106">**Кнопка збереження шаблону сайту або списку недоступна або відсутня**</span><span class="sxs-lookup"><span data-stu-id="57d6d-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="57d6d-107">Адміністраторам потрібно дозволити настроюваний сценарій для ввімкнення функцій шаблону.</span><span class="sxs-lookup"><span data-stu-id="57d6d-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="57d6d-108">Докладні вказівки, приклади та міркування див.</span><span class="sxs-lookup"><span data-stu-id="57d6d-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="57d6d-109">Дозволити або заборонити настроюваний сценарій</span><span class="sxs-lookup"><span data-stu-id="57d6d-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="57d6d-110">Команда "зберегти сайт як шаблон" не підтримується та може спричинити проблеми на сайтах, які використовують інфраструктуру публікування SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="57d6d-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="57d6d-111">**Не вдалося створити шаблон сайту або не працює належним чином**</span><span class="sxs-lookup"><span data-stu-id="57d6d-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="57d6d-112">Можливо, у шаблоні немає [функції](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , і його не активовано.</span><span class="sxs-lookup"><span data-stu-id="57d6d-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="57d6d-113">Якщо функція недоступна для активації в поточній колекції сайтів, шаблон сайту не можна використовувати для створення сайту.</span><span class="sxs-lookup"><span data-stu-id="57d6d-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="57d6d-114">Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) в пунктах 5000, оскільки це може заблокувати створення шаблону сайту.</span><span class="sxs-lookup"><span data-stu-id="57d6d-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="57d6d-115">Сайт може використовувати забагато ресурсів, тому шаблон сайту перевищує граничну кількість 50 МБ.</span><span class="sxs-lookup"><span data-stu-id="57d6d-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="57d6d-116">Під час відображення даних зі списку, у якому використовується стовпець підстановки, виникають проблеми.</span><span class="sxs-lookup"><span data-stu-id="57d6d-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="57d6d-117">Щоб отримати докладніші відомості, [у списку в службі SharePoint Online не відображаються дані зі списку правильних підстановок](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="57d6d-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="57d6d-118">Щоб отримати докладні відомості про поширені проблеми та рішення, перевірте [створення та використання шаблонів сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="57d6d-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



