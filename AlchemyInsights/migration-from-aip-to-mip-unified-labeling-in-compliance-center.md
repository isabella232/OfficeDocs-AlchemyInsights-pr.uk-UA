---
title: Перенесення з AIP до MIP/уніфікованого маркування в центрі відповідності
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674347"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Перенесення з AIP до MIP/уніфікованого маркування в центрі відповідності

Щоб перенести з міток AIP до уніфікованого маркування в центрі безпеки та відповідності, виконайте наведені нижче дії.

**Активація захисту від порталу "Лазурний"**

1. Якщо ви ще не зробили цього, відкрийте нове вікно браузера та [ввійдіть на порталі Azure](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Перейдіть на відповідне лезо для **захисту інформації** . Наприклад, у меню "концентратор" виберіть пункт **Усі служби** та починайте вводити **дані** в полі фільтра. Виберіть пункт **захист інформації з Azure**. Якщо ви ще не отримували відповідь на захист інформації в Лазурне, перегляньте один раз [додаткові кроки](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , щоб додати цей Клинок до порталу. Щоб відкрити відповідний елемент захисту від Блакитної інформації, необхідно мати [або план](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) Office 365, який включає в себе керування правами. Якщо у вас є одна з цих передплат, але відображається повідомлення про те, що дійсна Передплата не знайдена, [зверніться до служби підтримки Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) або скористайтеся стандартними каналами підтримки.

2. Знайдіть пункти меню **керування** , а потім виберіть пункт **Активація захисту**. Натисніть кнопку **активувати**, а потім підтвердьте дію. Після завершення активації інформаційна панель відображає **активацію успішно завершено**.

**Перенесення міток захисту даних Azure до центру відповідності & безпеки Office 365**

1. Переконайтеся, що ви ввійшли як користувач із дозволом глобального адміністратора.

2. Перейдіть на відповідне лезо для **захисту інформації** .

3. У меню " **керування** " виберіть пункт " **уніфіковане маркування**".

4. На **Лазуркому захист інформації – єдиний відповідний** клинок, натисніть кнопку **активувати** та дотримуйтеся вказівок в Інтернеті.

**Зверніть увагу**: переконайтеся, що у вас є відповідні дозволи, перш ніж активувати перенесення центру безпеки & відповідність. Перегляньте ці статті, щоб отримати докладніші відомості.

1. [Чи потрібно мати Глобальний адміністратор для налаштування захисту інформації в Azure, чи можна делегувати інших адміністраторів?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Важлива інформація про адміністративні ролі після переходу до центру відповідності безпеки &.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Щоб отримати докладніші відомості про службу "AIP" для об'єднаного маркування в центрі безпеки та відповідності, перегляньте статтю [перенесення етикеток](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
