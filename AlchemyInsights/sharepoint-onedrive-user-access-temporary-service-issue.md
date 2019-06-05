---
title: Продуктивність питань SharePoint або OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719537"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint або OneDrive повільно, недоступних або недоступні для кількох користувачів

Якщо сайт OneDrive або SharePoint недоступний для декількох користувачів, які раніше мали доступ, може бути тимчасова служби питання. [Перевірте службу здоров'я приладної дошки](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Додати і Ліцензія користувача

Переконайтеся, що ви [призначити ліцензії для користувачів у службі Office 365 для бізнесу](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Призначте дозволи

Якщо користувач присвоїло Sharepoint ліцензії і як і раніше отримує повідомлення про відмову в доступі, переконайтеся, що вони мають [відповідний рівень дозволів](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) призначено.

## <a name="consider-using-the-access-request-feature"></a>Спробуйте використати функцію запиту доступу

[Запит доступу особливість](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) дозволяє людям запитують доступ до вмісту, що вони в даний час не мають дозволу переглядати.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Дозволити власний сценарій може викликати проблеми в доступі

Є певні сценарії, де функція *дозволити власний сценарій* може представляти в доступі. Список функцій, які постраждали, міркування безпеки та можливість вимкнути цю функцію. Будь ласка, відвідайте [дозволити або заборонити власний сценарій](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

