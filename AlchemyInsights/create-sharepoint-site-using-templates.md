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
# <a name="create-sharepoint-sites-using-templates"></a>Створення сайтів SharePoint за допомогою шаблонів

Можливість зберегти сайт як шаблон не підтримується на сучасних сайтах спілкування або груп. Докладні відомості про використання шаблонів наведено в статті [збереження, завантаження та передавання сайту SharePoint як шаблону](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Нижче наведено кілька поширених проблем і рішень щодо збереження сайту або списку як шаблону в службі SharePoint Online. 

**Кнопка збереження шаблону сайту або списку недоступна або відсутня**

Адміністраторам потрібно дозволити настроюваний сценарій для ввімкнення функцій шаблону. Докладні вказівки, приклади та міркування див. 

- [Дозволити або заборонити настроюваний сценарій](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Команда "зберегти сайт як шаблон" не підтримується та може спричинити проблеми на сайтах, які використовують інфраструктуру публікування SharePoint Server.

**Не вдалося створити шаблон сайту або не працює належним чином**

Можливо, у шаблоні немає [функції](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , і його не активовано. Якщо функція недоступна для активації в поточній колекції сайтів, шаблон сайту не можна використовувати для створення сайту.

- Перевірте, чи будь-які списки або бібліотеки перевищують [граничне значення обмеження подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) в пунктах 5000, оскільки це може заблокувати створення шаблону сайту.

- Сайт може використовувати забагато ресурсів, тому шаблон сайту перевищує граничну кількість 50 МБ.


- Під час відображення даних зі списку, у якому використовується стовпець підстановки, виникають проблеми. Щоб отримати докладніші відомості, [у списку в службі SharePoint Online не відображаються дані зі списку правильних підстановок](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Щоб отримати докладні відомості про поширені проблеми та рішення, перевірте [створення та використання шаблонів сайтів](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



