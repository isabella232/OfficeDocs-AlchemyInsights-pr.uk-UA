---
title: Створення сайту в SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b9009fdbdc2a5e7443151446daade1685d2f5d45
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770444"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="d2c66-102">Створення сайтів SharePoint за допомогою шаблонів</span><span class="sxs-lookup"><span data-stu-id="d2c66-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="d2c66-103">Можливість збереження сайту як шаблону не підтримується сучасними комунікаційними або веб-сайтами.</span><span class="sxs-lookup"><span data-stu-id="d2c66-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="d2c66-104">Для отримання додаткових відомостей про використання шаблонів дивіться [збереження, завантаження та завантаження сайту SharePoint як шаблону](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="d2c66-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="d2c66-105">Нижче наведено деякі поширені проблеми/рішення щодо збереження сайту або списку як шаблону в SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d2c66-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="d2c66-106">**Зберегти сайт/шаблон списку кнопка недоступна або відсутня**</span><span class="sxs-lookup"><span data-stu-id="d2c66-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="d2c66-107">Адміністраторам потрібно буде дозволити користувацький скрипт для ввімкнення функцій шаблону.</span><span class="sxs-lookup"><span data-stu-id="d2c66-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="d2c66-108">Докладні кроки, приклади та міркування див.</span><span class="sxs-lookup"><span data-stu-id="d2c66-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="d2c66-109">Дозволити або заборонити користувацький скрипт</span><span class="sxs-lookup"><span data-stu-id="d2c66-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="d2c66-110">Команда Зберегти як шаблон не підтримується і може спричинити проблеми на веб-сайтах, які використовують видавничу інфраструктуру SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="d2c66-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="d2c66-111">**Не вдалося створити шаблон сайту або не працює належним чином**</span><span class="sxs-lookup"><span data-stu-id="d2c66-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="d2c66-112">Можливо, шаблон відсутній, а [функція](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) не активується.</span><span class="sxs-lookup"><span data-stu-id="d2c66-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="d2c66-113">Якщо функція недоступна для активації в поточній колекції сайтів, не можна використовувати шаблон сайту для створення сайту.</span><span class="sxs-lookup"><span data-stu-id="d2c66-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="d2c66-114">Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 елементів, оскільки це може блокувати створення шаблону сайту.</span><span class="sxs-lookup"><span data-stu-id="d2c66-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="d2c66-115">Можливо, сайт використовує забагато ресурсів, і тому шаблон сайту перевищує ліміт 50 МБ.</span><span class="sxs-lookup"><span data-stu-id="d2c66-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="d2c66-116">Є проблеми з відображенням даних зі списку, який використовує стовпець підстановки.</span><span class="sxs-lookup"><span data-stu-id="d2c66-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="d2c66-117">Для отримання додаткових відомостей див. у [списку шаблон не відображаються дані зі списку правильні підстановки в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="d2c66-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="d2c66-118">Для отримання більш детальної інформації про типові проблеми та рішення, будь ласка, перевірте [Створюйте та використовуйте шаблони сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="d2c66-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



