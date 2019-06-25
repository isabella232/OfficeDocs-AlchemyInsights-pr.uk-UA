---
title: Створити сайт у SharePoint Online
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199294"
---
# <a name="create-sharepoint-sites-using-templates"></a>Створення сайтів SharePoint за допомогою шаблонів

Шаблони сайтів SharePoint є готові визначень призначені навколо потреби конкретного бізнесу. Докладніше перегляньте статтю [використання шаблонів для створення різних видів сайтів SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Нижче наведено деякі поширені питання/рішення щодо збереження через сайт або список як шаблон у Sharepoint Online. 

**Зберегти сайт/список шаблон кнопка не буде доступна або відсутні**

Адміністратори повинні дозволити користувацький скрипт для ввімкнення функції шаблон. Докладно процедуру описано приклади і міркування див 

- [Дозволити або заборонити власний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Сайт зберегти як шаблон команда не підтримується і може викликати проблеми на сайтах, які використовують Видавничий інфраструктури SharePoint Server.

**Шаблон сайту неможливо створити або працює неправильно**

Шаблон може бути відсутня [функція](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) і не буде активувати. Якщо функція недоступна для активації в поточній колекції сайтів, це неможливо використовувати шаблон сайту для створення сайту.

- Перевірте, якщо будь-які списки або бібліотеки перевищує [Ліміт граничне значення подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) з 5000 пунктів, як це може блокувати створення шаблон сайту.

- Можливо, сайт використовує забагато ресурсів і тому шаблон сайту перевищує обмеження в 50 МБ.


- Є проблеми відображення даних зі списку, який використовує стовпець підстановки. Докладніше перегляньте [створеного шаблону списку не відображаються дані зі списку правильний підстановки в SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).

Для більш докладної інформації про загальні проблеми і рішення будь ласка, перевірте [створення і використання шаблонів сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



