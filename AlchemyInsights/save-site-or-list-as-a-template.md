---
title: Зберегти як шаблон сайту або списку
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: a74d14f1743b9a016346f7bf0943523b1ab21f91
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551652"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="1b8ee-102">Зберегти як шаблон сайту або списку</span><span class="sxs-lookup"><span data-stu-id="1b8ee-102">Save site or list as a template</span></span>

<span data-ttu-id="1b8ee-103">Шаблони сайтів SharePoint є готові визначень призначені навколо потреби конкретного бізнесу.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="1b8ee-104">Докладніше перегляньте статтю [використання шаблонів для створення різних видів сайтів SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="1b8ee-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="1b8ee-105">Нижче наведено деякі поширені питання/рішення щодо збереження через сайт або список як шаблон у SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="1b8ee-106">**Зберегти сайт/список шаблон кнопку несе не доступні без вісті**.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="1b8ee-107">Адміністратори повинні дозволити користувацький скрипт для ввімкнення функції шаблон.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="1b8ee-108">Докладно процедуру, приклади і міркування в розділі [дозволити або заборонити власний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="1b8ee-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="1b8ee-109">Сайт зберегти як шаблон команда не підтримується і може викликати проблеми на сайтах, які використовують Видавничий інфраструктури SharePoint Server.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="1b8ee-110">**Шаблон сайту неможливо створити або працює неправильно**</span><span class="sxs-lookup"><span data-stu-id="1b8ee-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="1b8ee-111">Шаблон може бути відсутня [функція](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) і не буде активувати.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="1b8ee-112">Якщо функція недоступна для активації в поточній колекції сайтів, це неможливо використовувати шаблон сайту для створення сайту.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="1b8ee-113">Перевірте, якщо будь-які списки або бібліотеки перевищує [Ліміт граничне значення подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) з 5000 пунктів, як це може блокувати створення шаблон сайту.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="1b8ee-114">Можливо, сайт використовує забагато ресурсів і тому шаблон сайту перевищує обмеження в 50 мегабайт (МБ).</span><span class="sxs-lookup"><span data-stu-id="1b8ee-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="1b8ee-115">Є проблеми відображення даних зі списку, який використовує стовпець підстановки.</span><span class="sxs-lookup"><span data-stu-id="1b8ee-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="1b8ee-116">Докладніше перегляньте [створеного шаблону списку не відображаються дані зі списку правильний підстановки в SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="1b8ee-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="1b8ee-117">Для більш докладної інформації про типові проблеми та рішення будь ласка посилання, [створення і використання шаблонів сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="1b8ee-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

