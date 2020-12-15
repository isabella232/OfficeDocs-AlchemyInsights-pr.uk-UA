---
title: Увімкнення керування витратами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678776"
---
# <a name="enable-cost-management"></a>Увімкнення керування витратами

**Що означає "витрати відключені для організації"?**

Організації за допомогою корпоративної угоди (EA) або облікових записів Microsoft для клієнтів (MCA) можуть забороняти доступ до відомостей про витрати та цінової інформації.

Після входу на портал Azure, вони можуть використовувати API для виставлення рахунків для програмного отримання рахунків-фактур (після того, як вони ввімкнув) і відомості про використання.

**Надання іншим користувачам доступу до рахунків-фактур**

1. Перейдіть на сторінку з відповідними **передплатою** на порталі Azure Portal.
2. Виберіть пункт **рахунки-фактури** , а потім – **доступ до рахунків-фактур**.
3. Увімкніть доступ, а потім збережіть зміни, щоб дозволити користувачам використовувати ролі на основі передплатою для завантаження рахунків-фактур.

> [!NOTE]
> Адміністратор облікового запису може також настроїти для надсилання рахунків-фактур електронною поштою. Щоб дізнатися більше, перегляньте статтю [отримання рахунка-фактури в електронному листі](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).

**Додавання користувачів до ролі невізуального рахунка**

1. Перейдіть на сторінку з відповідними **передплатою** на порталі Azure Portal.
2. Виберіть **елемент керування доступом (IAM)** , а потім натисніть кнопку **Додати**.
3. Виберіть елемент **невізуальний пристрій для виставлення рахунків** на сторінці **Виберіть роль** .
4. Введіть повідомлення електронної пошти користувача, якого потрібно запросити, а потім натисніть кнопку **OK** , щоб надіслати запрошення.
5. Виконайте вказівки, наведені в запрошенні електронної пошти, щоб увійти в систему як невізуальний пристрій для виставлення рахунків. Докладні відомості наведено в статті [надання доступу до рахунків](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).

**Рекомендовані документи**

- [Увімкнення подання "да" та "Ао" за допомогою порталу EA](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [Витрати, включені в керування витратами](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [Підтримувані пропозиції Microsoft Azure](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [Перевірка витрат у аналізі витрат](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [Надання доступу до відомостей для виставлення рахунків](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Перевірка доступу до угоди клієнта Microsoft](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






