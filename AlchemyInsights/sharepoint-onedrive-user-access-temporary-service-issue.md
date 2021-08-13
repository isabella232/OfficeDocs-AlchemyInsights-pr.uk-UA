---
title: Проблеми з продуктивністю SharePoint або OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093869"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint або повільний OneDrive, недоступний або недоступний для кількох користувачів

Якщо певний OneDrive або SharePoint сайт недоступний для кількох користувачів, які раніше мали доступ, може виникнути тимчасова проблема з обслуговуванням. [Перевірте приладну дошку справності служби.](https://portal.office.com/adminportal/home#/servicehealth)

**Додавання та ліцензування користувача**

Переконайтеся, [що ви призначаєте ліцензії користувачам у Microsoft 365 для бізнесу.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Призначення дозволів**

Якщо користувачу призначено ліцензію SharePoint і користувач отримує повідомлення про відхилення доступу, переконайтеся, що користувачу призначено [відповідний](https://docs.microsoft.com/sharepoint/understanding-permission-levels) рівень дозволів.

**Рекомендовано використовувати функцію запитів на доступ**

Функція [запиту на доступ](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) дає змогу користувачам надсилати запити на доступ до вмісту, для перегляду яких у них зараз немає дозволу.

**Дозволити користувацькі сценарії можуть спричинити проблеми з доступом**

Деякі сценарії дають *змогу* за допомогою функції "Дозволити користувацькі сценарії" відхилити доступ. Список функцій, на які це впливає, з огляду на безпеку та можливість вимкнути цю функцію. Відвідайте [сторінку Дозвольте або забороніть користувацькі сценарії](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

