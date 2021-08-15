---
title: Проблеми з API Graph Microsoft
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975914"
---
# <a name="microsoft-graph-api-issues"></a>Проблеми з API Graph Microsoft

Ця стаття також може застосовуватися до розробників, які продовжують використовувати Azure AD Graph API. Проте ми **наполегливо** рекомендуємо використовувати Microsoft Graph для всіх сценаріїв керування каталогами, ідентичностями та доступом.

**Проблеми з автентифікацією або авторизацією**

- Якщо програмі  не вдається отримати маркери для виклику в Microsoft Graph, виберіть елемент Проблема з отриманням маркера доступу **(автентифікації)** категорії Microsoft Graph, щоб отримати конкретнішу довідку та підтримку з цієї статті.
- Якщо під час виклику Microsoft Graph надходять помилки авторизації **401 або 403,** виберіть категорію Отримання помилки **(авторизації)** Microsoft Graph API, щоб отримати конкретнішу довідку та підтримку з цієї статті.

**Я хочу використовувати програму Microsoft Graph, але не знаєте, з чого почати**

- [Огляд програми Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Огляд ідентичності та керування доступом у Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Початок роботи з програмами Microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – перевірка API Graph Microsoft у вашому клієнта або демонстрацією клієнта

**Я хочу використовувати Microsoft Graph але чи підтримується мені API каталогів v1.0?**

Microsoft Graph API для керування каталогами, ідентичноями та доступом. Проте між можливими розгалужень в Azure AD та Microsoft Graph і microsoft Graph. Перегляньте наведені нижче статті, у яких наведено найновіші відмінності, які можуть допомогти у виборі.

- [Відмінності між типами ресурсів між Azure AD Graph і Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Відмінності властивостей між Azure AD Graph і Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Відмінності між Azure AD та Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Інтерфейс API, з якого я викликаю, не працює. Де можна виконати додаткові перевірки?**

**Microsoft Graph Explorer.** Тестуйте API-Graph Microsoft у вашому клієнта або демонстрацією клієнта,  а також перегляньте зразки запитів у Microsoft Graph Explorer.

**Моя програма задовга, і вона також дроселюється. Які вдосконалення можна вдосконалити?**

Залежно від сценарію у вашому розпорядженні багато варіантів, щоб програма стала більш функціональною, і в деяких випадках служба може зменшити дроселяці (у разі завеликої кількості викликів).

- [Практичні Graph microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Запити на пакети](https://docs.microsoft.com/graph/json-batching)
- [Відстеження змін за допомогою запиту на видалення](https://docs.microsoft.com/graph/delta-query-overview)
- [Отримання сповіщення про зміни за допомогою веб-хостингу](https://docs.microsoft.com/graph/webhooks)
- [Указівки з керування регуляруванням](https://docs.microsoft.com/graph/throttling)

**Де можна знайти докладні відомості про помилки та відомі проблеми?**

- [Відомості про Graph про помилки в microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Відомі проблеми з microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Де можна перевірити стан доступності служби та підключення?**

Доступність і підключення відповідних служб, доступ до яких можна отримати через службу Microsoft Graph, може вплинути на загальну доступність і продуктивність microsoft Graph.

- Щоб Azure Active Directory відомості про справність служби, перевірте стан служб **безпеки та** ідентичності, перелічених на [сторінці стану Azure.](https://azure.microsoft.com/status/)
- Щоб Office служби, які вносяться в корпорації Майкрософт Graph, перевірте стан служб, перелічених на [приладні дошці справності](https://portal.office.com/adminportal/home#/servicehealth)служб Office служб.

Помилки авторизації Graph Microsoft можуть спричиняти кілька різних проблем, більшість із яких починають помилку 401 або 403. Наприклад, усі вони можуть призвести до помилок авторизації:

- Неправильні [потоки отримання маркерів доступу](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Неналежне налаштування [областей дозволів](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Відсутність [дозволу](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Припинення підтримки бібліотек Azure Active Directory автентифікації (ADAL) і Azure AD Graph API (AAD Graph)***

**З 30 червня 2020** р. ми більше не додаватимемо нові функції до ADAL і Azure AD Graph. Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.

**З 30 червня 2022** року ми завершимо підтримку ADAL і Azure AD Graph і більше не надаватимемо технічну підтримку або оновлення системи безпеки.

Програми, які використовують ADAL у наявних версіях ОС, і надалі працюватиме після цього, але не отримуватимете *технічної підтримки або оновлень системи безпеки.*

Програми, які використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки Azure AD Graph.

**Перенесення ADAL**

Ми радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.

Якщо ви використовуєте програми Microsoft, зверніть увагу, що корпорація Майкрософт зараз переносить свої програми до служби MSAL до крайніх термінів припинення підтримки, забезпечуючи переваги постійного захисту та вдосконалення функцій MSAL.

1. [Запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Дізнайтеся, як перенести програми платформами](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Якщо вам потрібна допомога з розумінням того, які програми використовують ADAL, радимо переглянути вихідний код усіх програм і, за потреби, зв'язатися з інтернет-провайдерами або постачальниками програм. Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому осередку.

**Перенесення AAD Graph**

Для програм, які використовують Azure AD Graph, дотримуйтеся наших вказівок, щоб [перенести програми Azure AD Graph до microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Контрольний список перенесення для початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. На порталі реєстрації Azure показано, які програми використовують AAD Graph. Радимо переглянути вихідний код усіх своїх програм і, за необхідності, зв’язатися з будь-якими незалежними постачальниками програмного забезпечення або постачальниками програм. Крім того, служба підтримки Microsoft може надати список усіх Graph AAD у вашому клієнтів.
3. Щоб програма отримла доступ до даних у Graph Microsoft, користувач або адміністратор повинен надати їй відповідні дозволи в процесі згоди. У [посиланні Graph дозволів Microsoft](https://docs.microsoft.com/graph/permissions-reference) на перелічено дозволи, пов'язані з кожним основним набором API-Graph Microsoft. Тут також наведено інструкції з використання дозволів.
