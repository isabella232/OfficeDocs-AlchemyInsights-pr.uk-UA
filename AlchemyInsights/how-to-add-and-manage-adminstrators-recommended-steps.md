---
title: Додавання адміністраторів і керування ними – рекомендовані дії
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339053"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Додавання адміністраторів і керування ними – рекомендовані дії

Ми знайшли рішення відповідно до опису вашої проблеми. Більшість клієнтів змогли самостійно вирішити проблему після перегляду нашої документації.

**Редагування адміністратора передплати або адміністратора**

- Адміністратор облікового запису може змінювати обидві ролі, тоді як адміністратор передплати може змінювати на порталі [Azure лише адміністратори.](https://ms.portal.azure.com/#home)
- [Додавання або змінення адміністраторів передплати Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Оновлення адміністратора передплати або передплати Co-Administrator внутрішніх (AIRS) передплат**

Адміністратор служби або адміністратор може самостійно виконати цю дію, виконавши такі дії:

1. Увійдіть [на портал Azure і клацніть](https://ms.portal.azure.com/#home) Керування **витратами + Виставлення** рахунків у лівій частині.
2. Клацніть позицію з передплатою. Відкриється огляд для вашої передплати.
3. На **надлишку** передплати клацніть **Властивості**. 
4. Натисніть кнопку **Адміністратор служби.**
5. Введіть адресу електронної пошти користувача, якого потрібно зробити адміністратором служби, і натисніть кнопку **OK.**

**Додавання, змінення або видалення спів адміністратора**

1. Увійдіть [на портал Azure](https://ms.portal.azure.com/#home) як адміністратор служби.
2. Відкрийте [розділ Передплати](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) та виберіть передплату. (Співадміністраторів можна призначати лише в області передплати.)
3. Перейдіть до класичних адміністраторів керування доступом **(IAM).** Додайте співадміні адміністратора, щоб відкрити область Додавання співавтора (якщо параметр Додати спільного адміністратора вимкнуто, це означає, що у вас немає  >    >    >   дозволів). 
4. Виберіть користувача, якого потрібно додати, і натисніть кнопку **Додати**.

**Дізнатися більше:**
- [Додавання співавра](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Вилучення співавра](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Змінення адміністратора служби](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Перегляд адміністратора облікових записів](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Керування доступом за допомогою порталу RBAC і Azure](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Додавання або видалення користувачів за Azure Active Directory (AD)**

Ви можете додати нових користувачів або видалити наявних із Azure Active Directory (Azure AD).

1. Щоб додати нового користувача, увійдіть на портал [Azure](https://ms.portal.azure.com/#home) як адміністратор користувача для організації.
2. Виберіть **Azure Active Directory** послідовно **виберіть елементи** Користувачі та **Новий користувач**.
3. На сторінці **Користувач** введіть потрібні відомості. Натисніть **кнопку Створити.** Користувача буде створено та додано до клієнта Azure AD.

**Докладні відомості:**

- [Додавання нового користувача](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Видалення користувача](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Додавання або оновлення відомостей профілю користувача за допомогою Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Рекомендовані документи**

- [Що таке керування доступом на основі ролей (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Різні ролі в Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Дозволи на роль адміністратора в Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Навчальна вправа: надання доступу для користувача за допомогою RBAC і порталу Azure](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Усунення несправностей, пов'язаних із RBAC в Azure](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Упорядкування ресурсів за допомогою груп керування Azure](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Як надіслати запит на копію рахунка-фактури з Azure електронною поштою](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Додавання, оновлення й видалення кредитної або дебетової картки в Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Керування передплатою (повторна активація, скасування або змінення передплати)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



