---
title: Підтримувані типи передплатою
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
- "9003560"
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807984"
---
# <a name="supported-subscription-types"></a>Підтримувані типи передплатою

Ознайомтеся з підтримуваними типами передплатою, щоб продовжити подальше.

[Підтримувані типи передплатою](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

**Передача права власності на виставлення рахунків**

Портал "Лазурний" як [адміністратор облікового](https://ms.portal.azure.com/) запису рахунка, який має передплатою, яку потрібно перенести.

- Пошук у службі **керування витратами + виставлення рахунків** . Виберіть пункт **передплати** з області ліворуч. Залежно від Access може знадобитися вибрати область виставлення рахунків, а потім **передплачений** або **блакитні передплати** .
- Виберіть пункт передати право власності на виставлення рахунків для передплатою, яку потрібно перенести.
- Введіть адресу електронної пошти користувача, який є адміністратором виставлення рахунків, який стане новим власником для передплатою, а потім натисніть кнопку **Надіслати запит на перенесення**
- Користувач отримує повідомлення електронної пошти з інструкціями, щоб переглянути ваш запит на перенесення. Щоб затвердити запит на перенесення, користувач вибирає посилання в електронному листі та відповідає інструкціям.

Примітка. Якщо ви переносите право власності на ваш обліковий запис для облікового запису користувача в іншому клієнті Azure AD, усі завдання, які [базуються на рольовій службі керування доступом (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) для керування ресурсами в передплаті, остаточно видалено. Лише новий власник матиме доступ до керування ресурсами в передплаті. Докладні відомості наведено в статті [передавання передплатою користувачу в іншому клієнті Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

**Передача права власності на передплачений**

Права на доступ до ресурсів, які передаються на основі прав власності на підключення (RBAC) для керування ресурсами в передплаті, втрачають доступ. Щоб отримати докладні відомості про те, як додати наявну абонентську плату до клієнта, перегляньте статтю [зв'язати або додати "Лазурний" до "Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)".

- Передача за передплатою з існуючою видатною сумою від поточного циклу рахунків не передаватиметься на новий платіжний інструмент у новому обліковому записі. Єдиною інформацією, доступною для користувачів у новому обліковому записі, є вартість останнього місяця для вашої передплатою. Решта історії використання та виставлення рахунків не передаються за передплатою.
- Перенесення права власності на корпоративні угоди (EA), які зараз підтримуються на порталі "корпоративні угоди"
- Щоб прийняти запит на передачу, як-от Visual Studio, BizSpark, Партнерська мережа Microsoft для нового користувача вимагає, щоб у новому користувачу було потрібно мати ліцензію на програму Visual Studio/Microsoft партнер Network.
- Усі ресурси, як-от віртуальні машини, диски та веб-сайти, передаються до нового облікового запису успішно. Ці ресурси можуть вплинути на передачу передплатою для перехресного компонента:

**Служби домену Azure AD**

Сховища "блакитні ключові"

- Можуть бути порушені [користувачі та бази даних SQL](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) , особливо якщо клієнт використовує відповідну автентифікацію за допомогою служби Azure Active Directory
- Облікові **служби** , настроєні за допомогою автентифікації Azure Active Directory, можуть бути порушені
- **Команда Visual Studio** Облікові записи служб, підключені до передплати на Azure, можуть тимчасово втратити доступ, коли передплату на підключену Azure буде скасовано.

**Рекомендовані документи**

Кроки після прийняття права власності на виставлення рахунків:

- Щоб зберегти право власності на виставлення рахунків, а також змінити тип своєї передплатою, зверніться до: змінення [передплатою "Лазурний" на іншу пропозицію](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Передача Visual Studio, Партнерська мережа Microsoft (MPN) і оплата під час переходу до dev/Test передплати](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Перерахування права власності на корпоративні угоди (EA)](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [Запитання й відповіді про права власності](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Усунення проблем із відповідним Передаваннями](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)