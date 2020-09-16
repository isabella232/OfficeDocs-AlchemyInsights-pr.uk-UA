---
title: Не відображаються позначки чутливості
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801205"
---
# <a name="sensitivity-labels-not-appearing"></a>Не відображаються позначки чутливості

Позначки чутливості дають змогу класифікувати та захищати ваш чутливий вміст. Їх можна створити в центрі відповідності Microsoft 365, центрі безпеки Microsoft 365 або в центрі безпеки та конфіденційності Microsoft 365 & центр відповідності класифікації > Мітки чутливості. Докладні відомості про цю функцію наведено в статті [Огляд міток чутливості](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).

Якщо ви настроїли Мітки конфіденційності, але вони не відображаються в програмах Microsoft 365, установіть наведені нижче дії.

- Переконайтеся, що підпис "чутливість" [опубліковано](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) для користувачів і груп, які потрібно виконати.

- Переконайтеся, що користувач використовує програму, яка підтримує позначки чутливості, [у документі відображаються позначки чутливості](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).

- Якщо ви [мігруєте Мітки захисту від Блакитної інформації](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ознайомтеся з наведеними [тут](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)міркуваннями.

- Підтримка захисту від втрати даних (DLP): наразі можна використовувати лише Мітки збереження, як умову в політиці DLP.  Підтримка міток чутливості у політиці DLP недоступна, але ми працюємо над ним.

- Якщо функцію шифрування ввімкнуто на етикетці чутливості, можна вибрати один із таких варіантів:
    - Призначити дозволи зараз
    - Дозволити користувачам призначати дозволи


Докладні відомості про можливі проблеми наведено в статті [відомі проблеми з підписами чутливості](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).