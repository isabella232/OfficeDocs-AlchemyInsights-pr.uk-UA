---
title: Мітки чутливості не відображаються
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
ms.openlocfilehash: 824824257fee4aaaab1f2dd32597b4cdc858d035fabd357af90cf054dd35c9c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061453"
---
# <a name="sensitivity-labels-not-appearing"></a>Мітки чутливості не відображаються

Підписи чутливості дають змогу класифікувати та захистити ваш чутливий вміст. Їх можна створити в Центрі безпеки Центр відповідності Microsoft 365, Microsoft 365 або Microsoft 365 центрі безпеки & у розділі Класифікація > мітки конфіденційності. Докладні відомості про цю функцію див. в статтях Огляд підписів [чутливості.](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels)

Якщо ви налаштували підписи чутливості, але вони не відображаються в програмах Microsoft 365, перевірте таке:

- Переконайтеся, що підпис чутливості опубліковано [для](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) потрібних користувачів і груп.

- Переконайтеся, що користувач використовує програму, що підтримує мітки чутливості, – див. мітки чутливості [в документі.](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)

- У разі [перенесення етикеток](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)захисту даних Azure слід враховувати перелічені [тут рекомендації.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)

- Підтримка захисту від втрати даних (DLP). Наразі в політиках DLP можна використовувати лише підписи збереження.  Підтримка підписів конфіденційності в політиці DLP ще не доступна, але ми працюємо над нею.

- Якщо для підпису чутливості ввімкнуто шифрування, можна вибрати один із цих варіантів:
    - Призначити дозволи зараз
    - Надання користувачам дозволів


Докладні відомості про можливі проблеми див. в сторінці Відомі проблеми з підписами [чутливості.](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)