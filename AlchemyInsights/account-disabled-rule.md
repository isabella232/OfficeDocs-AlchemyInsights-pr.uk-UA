---
title: Правило вимкнення передплати або облікового запису
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003559"
- "6676"
ms.openlocfilehash: 8918b0da0172e0421ade6f0cca936e14d1d609896bc4c75c5a8491c0dbe75aff
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938464"
---
# <a name="azure-subscription-disabled"></a>Передплату Azure вимкнуто

Передплату на Azure можна вимкнути, тому що минув термін дії вашої кредитної картки, ви досягли ліміту витрат, виставили прострочені рахунки, перевищили граничну суму кредитної картки або через те, що передплату скасував адміністратор облікового запису. Нижче описано, як можна повторно ввімкнути передплату. Докладні відомості: [Повторна активація передплати Azure](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support)

**Повторне ввімкнення передплати на Azure (передплату випадково скасовано)** Адміністратор [облікового запису](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa) може повторно активувати скасовану передплату на Pay-As-You-Go в Центрі облікових записів:

1. Увійдіть у [Центр облікових записів.](https://account.windowsazure.com/Subscriptions)
2. Виберіть скасовану передплату. Натисніть **кнопку Повторна активація**.

Щоб отримати відомості про інші [типи](https://portal.azure.com/?#blade/Microsoft_Azure_Support/HelpAndSupportBlade) передплат, зверніться до служби підтримки, щоб повторно активувати передплату.

**Кредитна картка з простроченим терміном дії**

Під час реєстрації безкоштовного облікового запису **Azure** ви отримуєте безкоштовну ознайомлювальну передплату, яка надає вам 200 дол. США в кредитах Azure протягом 30 днів і 12 місяців безкоштовних служб. Наприкінці 30 днів Azure вимикає передплату. Вашу передплату вимкнуто, щоб захистити вас від випадкових стягнення плат за використання поза межами кредиту та безкоштовних служб, включених до вашої передплати. Щоб продовжити використовувати служби Azure, потрібно [оновити передплату](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support). Після оновлення передплата ще має доступ до безкоштовних служб протягом 12 місяців. Плату буде стягнуто лише за використання поза межами безкоштовних служб і кількості.  
Докладні відомості: [Кредитна картка, термін дії яких завершився](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable?WT.mc_id=Portal-Microsoft_Azure_Support#your-credit-is-expired)

**Досягнуто ліміту витрат**

Коли ви досягнете ліміту витрат, Azure вимикає передплату протягом решти періоду виставлення рахунків. Вашу передплату вимкнуто, щоб захистити вас від випадково стягнення плати за використання поза межами кредиту, включеного до вашої передплати. Відомості про вилучення ліміту витрат див. в [цьому списку.](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)  
Докладні відомості: [Досягнуто обмеження витрат](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled?WT.mc_id=Portal-Microsoft_Azure_Support#you-reached-your-spending-limit)

**Прострочений платіж**

Відомості про прострочені кошти див. в статті Усунення простроченого залишку для передплати Azure після отримання [повідомлення електронної пошти з Azure](https://docs.microsoft.com/azure/billing/billing-azure-subscription-past-due-balance?WT.mc_id=Portal-Microsoft_Azure_Support).

**Перевищення граничної кількості кредитних карток**

Щоб вирішити цю проблему, [перейдіть на іншу кредитну картку](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support). Або, якщо ви представляєте бізнес, ви можете перейти до оплати [за рахунком-фактурою](https://docs.microsoft.com/azure/billing/billing-how-to-pay-by-invoice?WT.mc_id=Portal-Microsoft_Azure_Support).

**Примітка.** Новій ювілейній термін дії передплати призначається повторно активовані передплати. Кількість днів (інтервал), у якому призупинено передплату, буде додано до вихідної дати пакета оновлення. Будь-яка дата річниці, що припадають на 29, 30 або 31-й, призведе до встановлення дати 1-го, наступного місяця.  
Приклад.

- Ваша вихідна ювілейна передплата – 25-й;
- Передплату призупинено 3 грудня 2010 р. і знову ввімкнуто 10.09.
- Передплату вимкнуто протягом 6 днів (інтервал 6);
- Після цього інтервал додається до вихідного коду sa, а сума стане новою датою sa (25+6=31). 

**Примітка.** У цьому прикладі, оскільки дата ДАТИ обслуговування перевищує 28, нова дата ДАТИ ОБСЛУГОВУВАННЯ буде 1-й наступного місяця.

**Рекомендовані документи**

- [Зміна передплати](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Скасувати передплату](https://docs.microsoft.com/azure/billing/billing-how-to-cancel-azure-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)  
- [Ринок Azure](https://azuremarketplace.microsoft.com/marketplace/?source=datamarket)
- Пошук адміністратора [облікових записів](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- [Що робити, якщо передплату На Azure вимкнуто?](https://docs.microsoft.com/azure/billing/billing-subscription-become-disable/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Обмеження витрат в Azure](https://docs.microsoft.com/azure/cost-management-billing/manage/spending-limit?WT.mc_id=Portal-Microsoft_Azure_Support)
