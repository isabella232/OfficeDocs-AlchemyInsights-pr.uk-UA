---
title: Додавання та керування adminstrators-рекомендованими кроками
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
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678867"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Додавання та керування adminstrators-рекомендованими кроками

**Редагування адміністратора або Співадміністратора за передплатою**

- Адміністратор облікового запису може редагувати обидві ролі, якщо адміністратор передплатникам може змінити лише один із адміністраторів на [порталі Azure](https://ms.portal.azure.com/#home).
- [Додавання або змінення адміністраторів служби Azure передплатникам](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Оновлення адміністратора передплати або Co-Administrator для передплати на внутрішні (КОНДИЦІОНУВАННЯ)**

Адміністратор служби або спільний адміністратор може самостійно обслуговувати цю дію, виконавши наведені нижче дії.

1. Увійдіть на [портал Azure](https://ms.portal.azure.com/#home) і клацніть елемент **керування витратами + виставлення рахунків** у лівому клинку.
2. Клацніть елемент з передплатою. Відкриється огляд вашої передплатою.
3. На клинку **передплатою** натисніть кнопку **Властивості**. 
4. Натисніть кнопку **адміністратор служби** .
5. Укажіть повідомлення електронної пошти користувача, якого потрібно встановити як адміністратор служби, і натисніть кнопку **OK**.

**Додавання та змінення та видалення Співадміністратора**

1. Увійдіть на портал " [Лазурний](https://ms.portal.azure.com/#home) " як адміністратор служби.
2. Відкрийте [передплату та виберіть передплату.](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) (Adminstrators можна призначати лише в області "Передплата".)
3. Перейдіть до **елемента керування доступом (IAM)**  >  **Classic адміністратори**  >  **додайте** елемент  >  **Додати** до адміністратора, щоб відкрити область **Додавання спільного адміністратора** (якщо параметр Add Co-адміністратор вимкнуто, це означає, що у вас немає дозволів).
4. Виберіть користувача, якого потрібно додати, і натисніть кнопку **Додати**.

**Дізнатися більше:**
- [Додавання спільної адміністратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Видалення співадміністратора](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Змінення адміністратора служби](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Перегляд адміністратора облікового запису](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Керування доступом за допомогою RBAC і Лазуропорталу](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Додавання та видалення користувачів за допомогою служби Azure Active Directory (AD)**

Ви можете додавати нових користувачів або видаляти вже доступні користувачі з організації Azure AD Active Directory:

1. Щоб додати нового користувача, увійдіть на [портал Azure](https://ms.portal.azure.com/#home) , як адміністратор користувача для організації.
2. Виберіть пункт " **Лазурний**", виберіть **користувачі** , а потім натисніть кнопку **створити користувача**.
3. На сторінці **користувача** заповніть необхідну інформацію. Натисніть кнопку **створити**. Користувач створюється та додається до свого клієнта Azure AD.

**Додаткові відомості**:

- [Додавання нового користувача](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Видалення користувача](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Додавання або оновлення відомостей профілю користувача за допомогою служби Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Рекомендовані документи**

- [Що таке елемент керування доступом на основі ролей (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Розуміння різних ролей у Azure](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Дозволи на роль адміністратора в "Лазурний" Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Навчальний посібник: надання доступу для користувача за допомогою RBAC та порталу "Лазурний"](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Усунення несправностей у RBAC в лазуровий](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Упорядкування ресурсів за допомогою «лазуровий груп керування»](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Запит на копіювання за допомогою електронної пошти копії Лазур-рахунка](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Як додати, оновити або видалити кредитну або дебетову картку з Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Керування (Повторна активація/скасування або переключення)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



