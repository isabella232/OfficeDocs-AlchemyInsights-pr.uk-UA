---
title: Передача прав власності на виставлення рахунків за Azure
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
- "6849"
ms.openlocfilehash: 74b7cc879973790b7532106c80b718856682a334
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755568"
---
# <a name="transfer-azure-billing-ownership"></a>Передача прав власності на виставлення рахунків за Azure

Увійдіть на [портал Microsoft Azure](https://portal.azure.com/) як адміністратор облікового запису для виставлення рахунків, де міститься потрібна передплата. Якщо ви не впевнені, чи маєте права адміністратора, або вам потрібно дізнатися, хто ним є, перегляньте статтю [Визначення адміністратора виставлення рахунків для облікового запису](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).

1. Введіть у пошуку _Керування витратами + виставлення рахунків_.
1. На панелі ліворуч виберіть **Передплати**. Залежно від типу доступу, можливо, потрібно буде спершу вибрати область виставлення рахунків, а потім натиснути **Передплати** або **Передплати Azure**.
1. Виберіть параметр **Передати права власності на виставлення рахунків** для потрібної підписки.
1. Введіть адресу електронної пошти користувача, який є адміністратором виставлення рахунків для облікового запису та буде новим власником передплати, і виберіть **Надіслати запит на передачу**.
1. Користувач отримає електронний лист із вказівками переглянути запит на передачу. Щоб схвалити його, користувач має натиснути посилання в листі та виконати вказівки.

Зверніть увагу: якщо ви передаєте права власності на підписку обліковому запису користувача в іншому осередку Microsoft Azure AD, усі призначення [керування доступом на основі ролей](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) для керування ресурсами в передплаті буде видалено назавжди. Лише новий власник зможе керувати ресурсами в передплаті. Щоб дізнатися, як змінити каталог для передплати, перегляньте статтю [Передача підписки користувачу в іншому осередку Microsoft Azure AD](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).

_**Важлива зміна у ваших рахунках-фактурах**_: якщо ви передали права власності на виставлення рахунків за підписку Azure, нарахування будуть розподілені пропорційно. Щоб отримати доступ до рахунків-фактур, виконайте дії нижче.  

1. Виберіть передплату на сторінці  [Передплати](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)  на порталі Microsoft Azure (у вас повинен бути  [доступ до рахунків-фактур](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)). Після цього виберіть  **Рахунки-фактури**.
1. Натисніть  **Завантажити рахунок-фактуру** , щоб переглянути копію рахунка-фактури у форматі PDF. Якщо з’явилося повідомлення  _Недоступно_, перегляньте розділ  [Чому я не бачу рахунок-фактуру за останній розрахунковий період?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)
1. Ви також можете переглянути інформацію про щоденне використання. Натисніть **розрахунковий період**, щоб завантажити PDF-файл із рахунком-фактурою та копію файлу (у форматі .csv) з докладними даними про щоденне використання. Щоб дізнатися більше, перегляньте статтю  [Як отримати рахунок-фактуру та дані про використання](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).

**Рекомендовані документи**

- [Передача прав власності на передплату Azure іншому обліковому запису](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [Про передачу прав власності на виставлення рахунків за передплату Azure](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [Передача підписок Visual Studio, Microsoft Partner Network (MPN) і Розробка й тестування з оплатою по факту використання](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [Запитання й відповіді про передачу прав власності](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [Усунення проблем із передачею прав власності](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
