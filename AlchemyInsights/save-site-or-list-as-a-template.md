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
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109225"
---
# <a name="save-site-or-list-as-a-template"></a>Збереження сайту або списку як шаблону

SharePoint сайтів – це попередньо створені визначення, призначені для певних бізнес-потреб. Докладні відомості [див. в статті Створення різних типів сайтів](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)за допомогою SharePoint шаблонів.

Нижче наведено кілька поширених проблем і рішень зі статті Збереження сайту або списку як шаблону у веб-SharePoint Online.

**Кнопка "Зберегти шаблон сайту або списку" недоступна або відсутня**. 

- Щоб активувати функції шаблонів, адміністраторам потрібно буде дозволити спеціальні сценарії. Докладні вказівки див. в статті Дозвіл і заборона користувацьких [сценаріїв.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Команда "Збереження сайту як шаблону" не підтримується та може призвести до проблем на сайтах, на яких використовується інфраструктура публікування SharePoint Server.


**Не вдалося створити шаблон сайту або він працює неправильно**

- Можливо, у шаблоні відсутня [функція,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) і його не вдається активувати. Якщо функція недоступна для активації в поточній колекції сайтів, ви не можете використовувати шаблон для створення веб-сайту.


- Перевірте, чи не перевищено в якихось списках або бібліотеках [обмеження для подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) в 5000 елементів, оскільки це може заважати створити шаблон.


- Можливо, сайт використовує забагато ресурсів, тому розмір шаблону сайту перевищує обмеження в 50 мегабайт (МБ).


- Існують проблеми з відображенням даних зі списку, у якому використовується стовпець підстановки. Докладні відомості [див. в статті Список,](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)створений за шаблоном, не відображає дані з правильного списку підстановки в SharePoint Online.


Докладніші відомості про поширені проблеми та способи їх вирішення див. в статті Створення [та використання шаблонів сайтів.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

