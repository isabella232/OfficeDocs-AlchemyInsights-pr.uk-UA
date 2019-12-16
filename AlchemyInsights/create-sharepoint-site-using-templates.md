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
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052490"
---
# <a name="create-sharepoint-sites-using-templates"></a>Створення сайтів SharePoint за допомогою шаблонів

Шаблони сайтів SharePoint – це заздалегідь створені визначення, створені навколо певної бізнес-потреби. Для отримання додаткових відомостей див. [використання шаблонів для створення різних типів сайтів SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Нижче наведено деякі поширені проблеми/рішення щодо збереження сайту або списку як шаблону в SharePoint Online. 

**Зберегти сайт/шаблон списку кнопка недоступна або відсутня**

Адміністраторам потрібно буде дозволити користувацький скрипт для ввімкнення функцій шаблону. Докладні кроки, приклади та міркування див. 

- [Дозволити або заборонити користувацький скрипт](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Команда Зберегти як шаблон не підтримується і може спричинити проблеми на веб-сайтах, які використовують видавничу інфраструктуру SharePoint Server.

**Не вдалося створити шаблон сайту або не працює належним чином**

Можливо, шаблон відсутній, а [функція](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) не активується. Якщо функція недоступна для активації в поточній колекції сайтів, не можна використовувати шаблон сайту для створення сайту.

- Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 елементів, оскільки це може блокувати створення шаблону сайту.

- Можливо, сайт використовує забагато ресурсів, і тому шаблон сайту перевищує ліміт 50 МБ.


- Є проблеми з відображенням даних зі списку, який використовує стовпець підстановки. Для отримання додаткових відомостей див. у [списку шаблон не відображаються дані зі списку правильні підстановки в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Для отримання більш детальної інформації про типові проблеми та рішення, будь ласка, перевірте [Створюйте та використовуйте шаблони сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



