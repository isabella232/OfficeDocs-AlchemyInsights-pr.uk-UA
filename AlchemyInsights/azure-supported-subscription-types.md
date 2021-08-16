---
title: Підтримувані типи передплати
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
- "9003560"
- "6675"
ms.openlocfilehash: f11eabdc18f708e34a6a10c67bc3e7416330cbf34aec20209b42252ffa0ab018
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072181"
---
# <a name="supported-subscription-types"></a>Підтримувані типи передплати

Перегляньте підтримувані типи передплати, щоб продовжити.

[Підтримувані типи передплати](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Передача прав на виставлення рахунків**

портал Microsoft Azure як [адміністратор облікового запису](https://ms.portal.azure.com/) для виставлення рахунків, що містить потрібну передплату

- Виконайте пошук у розділі **Керування витратами та виставлення рахунків**. Виберіть **Передплати** на панелі ліворуч. Залежно від типу доступу потрібно вибрати область виставлення рахунків, а потім натиснути **Передплати** або **Передплати на Azure**.
- Виберіть параметр "Передати права на виставлення рахунків" для потрібної передплати.
- Введіть адресу електронної пошти користувача, який є обліковим адміністратором облікового запису, у який буде перенесено передплату, і виберіть **Надіслати запит на передачу**
- Користувач отримає електронний лист із вказівками переглянути запит на передачу. Щоб схвалити його, користувач має натиснути посилання в листі та виконати вказівки.

Зверніть увагу: якщо ви передаєте права на виставлення рахунків за передплату обліковому запису користувача в іншому осередку Microsoft Azure AD, усі призначення в рамках [керування доступом на основі ролей](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) для керування ресурсами в передплаті буде остаточно вилучено. Лише новий власник зможе керувати ресурсами в передплаті. Докладні відомості див. в статті [Передача передплати користувачу в іншому осередку Microsoft Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Передача прав власності на передплату**

Під час передачі прав на передплату необхідні компоненти в рамках керування доступом на основі ролей для керування ресурсами в передплаті втратять доступ. Докладніше про додавання наявної передплати до осередку див. в статті [Зв’язування передплати Azure з Azure Active Directory або її додавання](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).

- Передплату з наявною сумою заборгованості в поточному циклі виставлення рахунків не буде переведено на новий платіжний засіб у новому обліковому записі. У новому обліковому записі користувачам буде доступна інформація лише про вартість передплати за останній місяць. Усі інші дані про використання та виставлення рахунків не буде перенесено разом із передплатою.
- Передача прав на виставлення рахунків для передплат за договором "Enterprise Agreement" наразі підтримується лише на порталі Enterprise Agreement
- Для передачі кредит-орієнтованої передплати, як-от Visual Studio, BizSpark, Microsoft Partner Network, новому користувачу необхідна ліцензія на Visual Studio або Microsoft Partner Network, щоб прийняти запит на передачу
- Усі ресурси, як-от віртуальні машини, диски та веб-сайти, переносяться в новий обліковий запис. Перенесення передплати з одного осередку в інший може вплинути на такі ресурси:

**Служба доменів Azure AD**

Сховища ключів Azure

- [Користувачі та бази даних, пов’язані з SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support), особливо якщо клієнт використовує автентифікацію, пов’язану з Azure Active Directory
- **Служби програм**, налаштовані з автентифікацією Azure Active Directory
- Облікові записи **Visual Studio Team Services**, підключені до передплат на Azure, можуть тимчасово втратити доступ у разі скасування підключеної передплати на Azure

**Рекомендовані документи**

Кроки після прийняття прав на виставлення рахунків

- Щоб зберегти права на виставлення рахунків, але змінити тип передплати, див. статті: [Перехід на іншу пропозицію передплати на Azure](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Перенесення передплат Visual Studio, Microsoft Partner Network (MPN) і передплат для розробки й тестування з оплатою по мірі використання](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Передача прав на виставлення рахунків для передплат за договором "Enterprise Agreement"](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Запитання й відповіді про передачу прав власності](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Усунення проблем із передачею прав власності](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)