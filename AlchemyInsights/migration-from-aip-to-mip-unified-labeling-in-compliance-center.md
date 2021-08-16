---
title: Перенесення З AIP на MIP/Unified Labeling у Центрі відповідності
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000387"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Перенесення З AIP на MIP/Unified Labeling у Центрі відповідності

Щоб перенести з етикеток AIP до пункту Уніфіковане підписування в Центрі безпеки та відповідності, виконайте такі дії:

**Активація захисту з порталу Azure**

1. Якщо ви цього ще не зробили, відкрийте нове вікно браузера та [ввійдіть на портал Azure.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Перейдіть до **лотка "Захист** даних в Azure". Наприклад, у меню Центр клацніть  Усі служби та почніть **вводити** дані в полі Фільтр. Виберіть **Захист даних в Azure**. Якщо ви раніше не отримували доступу до полотна "Захист [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) даних в Azure", див. одноразові додаткові дії з додавання цього блоку до порталу. Щоб відкрити ледь захист даних в Azure, потрібно мати план [Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) або план Office 365, який включає керування правами. Якщо у вас є одна з цих передплат, але відображається повідомлення про те, що не вдалося знайти дійсну передплату, зверніться до служби підтримки [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) або скористайтеся стандартними каналами підтримки.

2. Знайдіть **параметри меню Керування** та виберіть Захист **активація**. Натисніть **кнопку Активувати,** а потім підтвердьте дію. Коли активацію завершено, інформаційний рядок відображає вікно **Активацію успішно завершено.**

**Перенесення етикеток "Захист даних в Azure" Office 365 Центру безпеки & відповідності**

1. Переконайтеся, що ви ввійшли як користувач із дозволом глобального адміністратора.

2. Перейдіть до **лотка "Захист** даних в Azure".

3. У меню **"Керування"** виберіть пункт **Уніфіковане підписування**.

4. У **засобі "Захист даних в Azure – уніфікований надпис"** натисніть кнопку **Активувати** та дотримуйтеся вказівок в Інтернеті.

**Примітка.** Перш ніж активувати перенесення Центру відповідності &, переконайтеся, що у вас є відповідні дозволи. Докладні відомості див. в цих статтях:

1. [Чи потрібно вам глобальним адміністратором настроювати захист даних в Azure або делегувати іншим адміністраторам?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Важлива інформація про адміністративні ролі після перенесення до Центру безпеки & відповідності.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Докладні відомості про AIP до Центру безпеки та відповідності див. в цьому [центрі.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
