---
title: Створення сайту в SharePoint Online
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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057987"
---
# <a name="create-sharepoint-sites-using-templates"></a>Створення SharePoint сайтів за допомогою шаблонів

Можливість зберегти сайт як шаблон не підтримується для сучасних сайтів і сайтів команд. Додаткові відомості про шаблони див. в статті [Збереження, завантаження та передавання сайту SharePoint 2013 як шаблону](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Нижче наведено кілька поширених проблем і рішень щодо збереження сайту або списку як шаблону в SharePoint Online. 

**Кнопка "Зберегти шаблон сайту або списку" недоступна або відсутня**

Щоб активувати функції шаблонів, адміністраторам потрібно буде дозволити спеціальні сценарії. Докладні інструкції, приклади та рекомендації див. в цій статті. 

- [Дозвіл і заборона спеціальних сценаріїв](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Команда "Збереження сайту як шаблону" не підтримується та може призвести до проблем на сайтах, на яких використовується інфраструктура публікування SharePoint Server.

**Не вдалося створити шаблон сайту або він працює неправильно**

Можливо, у шаблоні відсутня [функція,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) і його не вдається активувати. Якщо функція недоступна для активації в поточній колекції сайтів, ви не можете використовувати шаблон для створення веб-сайту.

- Перевірте, чи не перевищено в якихось списках або бібліотеках [обмеження для подання списку](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) в 5000 елементів, оскільки це може заважати створити шаблон.

- Можливо, веб-сайт використовує занадто багато ресурсів, а тому шаблон веб-сайту перевищує обмеження в 50 МБ.


- Існують проблеми з відображенням даних зі списку, у якому використовується стовпець підстановки. Докладніше див. в статті [У списку, створеному за шаблоном, не відображаються дані з правильного списку підстановки у службі SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Докладніші відомості про поширені проблеми та способи їх вирішення див. в статті Створення [та використання шаблонів сайтів.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)



