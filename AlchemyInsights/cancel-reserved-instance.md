---
title: Скасування резервування
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
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819713"
---
# <a name="cancelling-reservation"></a>Скасування резервування

- **Самообслуговування:** Зарезервований екземпляр можна скасувати або обміняти самостійно [на порталі Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Виберіть резервування та натисніть кнопку "Відшкодування" або "Обмін". Зверніть увагу, що для обміну або відшкодування потрібно мати доступ власника до замовлення на резервування. Доступ лише до резервування не дозволяє продовжити відшкодування або обмін. Попросіть власника замовлення на резервування надати вам доступ до замовлення на резервування
- **Політика Exchange:** Ви можете обміняти резервування для іншого резервування того самого типу – при цьому немає жодних копій **на** обмін резервування. Загальне зобов'язання з новим резервуванням має бути більшим, ніж сума відшкодування коштів за обмін валюти та майбутні щомісячні платежі (якщо застосовно)
- **Політика відшкодування:** Сума відшкодування та скасовані майбутні платежі не можуть перевищувати 50 000 доларів США у 12-місячному вікні rolling window. **Наразі ми не стягуємо** пенсію під час відшкодування, але можемо стягувати її з майбутніх відшкодування.  
    **Винятки.** Можливість самостійного обміну та скасування передплати недоступна для клієнтів, укладених за договором "Us Government Enterprise Agreement"
- **Підтримка API, PS та CLI** недоступна для скасування та відшкодування самостійних обмінів і відшкодування для резервування [Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- Можливість самостійного обміну та скасування послуг недоступна для клієнтів, укладених за договором "Us Government Enterprise Agreement". Підтримуються інші типи передплат для державних установ США, зокрема Pay-As-You-Go і CSP.

Докладні відомості: [Як обробляються транзакції](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) повернення та обміну  
Докладні відомості: [Політики обміну та відшкодування](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
Інші запитання: ["Відвідати зарезервовані екземпляри для docs"](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange наявний зарезервований екземпляр (Self-service)**

Ви можете обмінюватися резервуваннями одного й того самого типу. Ви також можете відшкодувати резервування за рік до 50 000 доларів США, якщо воно більше не потрібне. Можливість самостійного обміну та скасування послуг недоступна для клієнтів, укладених за договором "Us Government Enterprise Agreement". Підтримуються інші типи передплат для державних установ США, зокрема Pay-As-You-Go і CSP. Щоб обмінятись або відшкодувати наявне резервування, потрібно мати доступ до замовлення власника.

Нижче описано процедуру завершення транзакції.

1. Увійдіть [на портал Azure.](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade) Виберіть резервування, які потрібно відшкодувати, і натисніть кнопку **Exchange**
2. Виберіть продукт віртуальної реальності, який потрібно придбати, і введіть кількість. Переконайтеся, що нова сума покупки перевищує загальну суму, що повертається, Перш ніж придбати, визначте [правильний розмір](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. Перегляд і виконання транзакції

**Відшкодування зарезервований екземпляр**

Щоб відшкодувати резервування, перейдіть до пункту **"Відомості** про резервування" та натисніть **"Відшкодування"**

**Пропорціонне відшкодування:**

**Приклади пропорційного та мінімального вимог щодо відшкодування та обміну**  
Приклад резервування на передньому плані:

- Придбано річний період RI за 120 дол. США з 1 січня
- 7 квітня ви хочете відшкодувати або обміняти це резервування
- Оскільки резервування проживає протягом 97 днів, ви отримаєте (1-97/365) * $120 назад. (наприклад, 88,1 дол. США). Наразі відшкодування не стягується
- Якщо нова покупка наради на суму перевищує 88,1 дол. США,
- Наразі відшкодування не стягується

**Приклад резервування плану виставлення рахунків:**

- Придбано річний термін дії RI за 10 дол. США на місяць
- 7 квітня ви хочете відшкодувати або обміняти це резервування
- Оскільки останній платіж відбувся 7 днів, ви отримаєте (1-7/31) * повернення 10 грн. (наприклад, 7,74 грн.)
- Майбутні платежі скасовано, – 80 дол. США. Наразі відшкодування не стягується
- Це скасування вирахує 87,74 дол. США з суми відшкодування в розмірі 50 000 грн.
- Якщо нова покупка змінна, загальна вартість нової покупки має бути більшою за 87,74 грн.

**Рекомендовані документи**

- [Спосіб обробки транзакцій повернення та обміну](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [Політики обміну та відшкодування](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)