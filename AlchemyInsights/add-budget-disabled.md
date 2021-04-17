---
title: Чому для мене вимкнуто кнопку "Додати бюджет"?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822656"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>Чому для мене вимкнуто кнопку "Додати бюджет"?

Щоб створити бюджет, знадобляться такі дозволи:

- Група керування, передплата, області груп ресурсів
- Contributor Керування витратами
- Власник
- Contributor
- Лише для корпоративних клієнтів: enrollment, Department, Account Scopes
- Адміністратор із проханням про зарахування (установити бюджет для області застосування даних)
- Адміністратор підрозділу (установлення бюджету в області підрозділу)
- Власник облікового запису (установлення бюджету в області бізнес-партнера)
- Лише сучасна клієнтська угода: обліковий запис для платних служб, профіль виставлення рахунків, області розділу рахунків
- Засіб для автора передплати Azure

**Бюджет створювався, коли витрати на поточний місяць уже перевибачено. Чому я не отримую оповіщення?**  
Якщо для створення бюджету вже перевищено граничне значення витрат, оповіщення не буде запущено. Коли новий цикл почнеться, якщо поламати порогові значення, оповіщення вимкнеться.

**Коли слід очікувати отримувати оповіщення після того, як перевищено одне з визначених граничних параметрів оповіщення про бюджет?**  
Бюджети обчислюються кожні 4 години. Щоб досягти системи бюджетів, дані про використання потрібно не менше 8 годин. З огляду на це, оповіщення можуть тривати до 12 годин після того, як буде перевищено граничне обмеження.

**Чому кнопку "Дата початку" вимкнуто, коли вибрано період скидання місяця або виставлення рахунків?**  
Бюджети вирівнюються за поточний календарний місяць або поточний розрахунковий період (у випадку, якщо вибрано «Місяць виставлення рахунків»). Тому ми попередньо заповнимо це значення для вас.

**Чому під час створення бюджету не відображається графік витрат?**  
Щоб створити графік, який допоможе створюватися бюджет, нам знадобиться дані про витрати щонайменше за 2 місяці.

**Чому не можна встановити бюджет для щойно створеної передплати?**  
Після створення передплати для обробки даних на обробку бюджету потрібно 24–48 годин.

**Бюджетні ресурси API**

- [Бюджети API по 1.](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)Дає змогу створювати й оновлювати бюджети. Використовуючи API бюджетів, ви можете встановити порогові значення бюджету та настроїти кілька оповіщень, щоб вони свільнялись під час наближення до цього порогу. Щоб автоматизувати оповіщення, можна ініціювати електронний лист або групу дій Azure. Примітка. Фільтрування для цього інтерфейсу API не вирівнює фільтрування або виміри query API.
- [Бюджети API v2.](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)Створення бюджетів із можливостями фільтрування більших витрат по v1. Фільтрування вирівнюватиметься за контрактом, який використовується в API-API запитів і вимірів. Ми рекомендуємо використовувати API бюджетів, щоб використовувати його вперед.
- [Розміри.](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)Дає змогу отримати підтримувані виміри для використання в різних областях. За допомогою API розмірів можна отримати список вимірів, які можна використовувати як вхідні дані для створення запитів за допомогою API запитів.
- [Запит.](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)Дає змогу отримувати сукупні дані про витрати та використання на основі запиту, який ви вказали. За допомогою API запиту можна вказати бажані параметри фільтрування, сортування та групування для всіх доступних вимірів (доступ до яких можна отримати за допомогою API вимірів).

**Прогнозовані витрати**

**Чому прогнози для витрат не бачать у аналізі витрат?**  
Прогнозування прогнозу в аналізі витрат може бути відсутнє з кількох причин:

1. Якщо ваші дані про витрати старіші за 10 днів, діаграма прогнозу не завантажиться. Модель вимагає принаймні 10 днів від нещодавніх даних про витрати для точного прогнозування
2. Якщо вибрано історичні дати, діаграма прогнозу не відображатиметься. Виберіть діапазон дат із майбутніми датами, щоб відобразити діаграму прогнозу
3. Якщо в обліковому записі є кілька грошових одиниць, на діаграмі прогнозу буде лише прогнозована вартість "Усі витрати в доларах США"

**Чому прогноз не змінюється під час внесення змін до ресурсів?**  
Щоб врахувати зміни в обліковому записі в прогнозованій моделі, потрібно кілька днів і негайно не вносити прогнози на основі змін у ресурсах.  
Щоб збільшити або зменшити ресурси, модель знайдить трохи більше часу, щоб врахувати їх для відміну від неї.

**Чому мій прогноз збільшується після того, як я зарезервую або придбаю Ринок?**  
Прогнозна модель врахує фактичні витрати та не враховує їх використання та придбання окремо. Для одноразового придбання модель зменшиться через 10 днів, щоб врахувати раптового збільшення витрат

**Потрібно переглянути прогнози для одного виміру (наприклад, Meter)**  
Прогноз наразі підтримує загальні прогнози витрат, а не для окремих метрів. Отже, коли вимір "Згруповано" буде згруповано, підсумовано всі елементи у вимірі.

**Рекомендовані документи**

- [Що таке Azure Cost Management?](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Практичні поради з Azure Cost Management](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Аналіз витрат і витрат](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Перегляд і аналіз витрат за допомогою аналізу витрат](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure Cost Management: Ціни](https://azure.microsoft.com/services/cost-management/#pricing)
- [Аналіз витрат в аналізі витрат](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [Відео. Створення бюджету на порталі Azure](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [Передумови для перегляду та настроювання бюджетів](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [Створення бюджетів і керування ними](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [Налаштування автоматизації за допомогою API груп дій і бюджетів Azure](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [Використання оповіщень про витрати для відстеження використання та витрат](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Практичні поради з керування витратами](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**Навчальні відео**

- [Створення бюджету на порталі Azure](https://go.microsoft.com/fwlink/?linkid=2146761)
- [Керування витратами за допомогою API бюджетів і груп дій](https://go.microsoft.com/fwlink/?linkid=2147038)