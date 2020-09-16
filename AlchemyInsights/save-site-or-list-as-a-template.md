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
# <a name="save-site-or-list-as-a-template"></a>Збереження сайту або списку як шаблону

Шаблони сайтів SharePoint – це попередньо створені визначення, розроблені навколо певної потреби бізнесу. Докладні відомості наведено в статті [використання шаблонів для створення різних типів сайтів SharePoint](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Нижче наведено кілька поширених проблем і рішень щодо збереження сайту або списку як шаблону в службі SharePoint Online.

**Кнопка збереження шаблону сайту або списку недоступна або відсутня**. 

- Адміністраторам потрібно дозволити настроюваний сценарій для ввімкнення функцій шаблону. Докладні вказівки, приклади та міркування [дають змогу переглянути або заборонити настроюваний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Команда "зберегти сайт як шаблон" не підтримується та може спричинити проблеми на сайтах, які використовують інфраструктуру публікування SharePoint Server.


**Не вдалося створити шаблон сайту або не працює належним чином**

- Можливо, у шаблоні немає [функції](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , і його не активовано. Якщо функція недоступна для активації в поточній колекції сайтів, шаблон сайту не можна використовувати для створення сайту.


- Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) в пунктах 5000, оскільки це може заблокувати створення шаблону сайту.


- Сайт може використовувати забагато ресурсів, тому шаблон сайту перевищує обмеження 50 мегабайт (МБ).


- Під час відображення даних зі списку, у якому використовується стовпець підстановки, виникають проблеми. Щоб отримати докладніші відомості, [у списку в службі SharePoint Online не відображаються дані зі списку правильних підстановок](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Щоб отримати докладні відомості про поширені проблеми та рішення, Дізнайтеся, як [створювати та використовувати шаблони сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

