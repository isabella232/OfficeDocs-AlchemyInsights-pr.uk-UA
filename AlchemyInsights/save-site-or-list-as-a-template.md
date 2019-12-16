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
# <a name="save-site-or-list-as-a-template"></a>Зберегти сайт або список як шаблон

Шаблони сайтів SharePoint – це заздалегідь створені визначення, створені навколо певної бізнес-потреби. Для отримання додаткових відомостей див. [використання шаблонів для створення різних типів сайтів SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Нижче наведено деякі поширені проблеми/рішення щодо збереження сайту або списку як шаблону в SharePoint Online.

**Зберегти сайт/шаблон списку кнопка недоступна або відсутня**. 

- Адміністраторам потрібно буде дозволити користувацький скрипт для ввімкнення функцій шаблону. Докладні кроки, приклади та [міркування див.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Команда Зберегти як шаблон не підтримується і може спричинити проблеми на веб-сайтах, які використовують видавничу інфраструктуру SharePoint Server.


**Не вдалося створити шаблон сайту або не працює належним чином**

- Можливо, шаблон відсутній, а [функція](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) не активується. Якщо функція недоступна для активації в поточній колекції сайтів, не можна використовувати шаблон сайту для створення сайту.


- Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000 елементів, оскільки це може блокувати створення шаблону сайту.


- Можливо, сайт використовує забагато ресурсів, і тому шаблон сайту перевищує ліміт 50 мегабайт (МБ).


- Є проблеми з відображенням даних зі списку, який використовує стовпець підстановки. Для отримання додаткових відомостей див. у [списку шаблон не відображаються дані зі списку правильні підстановки в SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Для отримання більш детальної інформації про загальні проблеми та рішення, будь ласка, посилання, [створювати і використовувати шаблони сайту](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

