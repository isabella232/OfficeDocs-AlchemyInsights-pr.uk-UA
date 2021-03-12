---
title: Проблеми з API Microsoft Graph
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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714518"
---
# <a name="microsoft-graph-api-issues"></a>Проблеми з API Microsoft Graph

Цей розділ може також застосовуватися до розробників, які ще використовують API Azure AD Graph. Однак **наполегливо** радимо використовувати Microsoft Graph для всіх сценаріїв служби каталогів, посвідчень та керування доступом.

**Проблеми з автентифікацією або авторизацією**

- Якщо ваша програма **не може придбати маркери** для виклику Microsoft Graph, виберіть **проблему з використанням маркера доступу (автентифікації)** Microsoft Graph, щоб отримати додаткову довідку й підтримку в цій статті.
- Якщо ваша програма **отримує 401 або 403 помилки авторизації** під час виклику Microsoft Graph, виберіть категорію **отримати доступ до помилки (авторизації)** Microsoft Graph API, щоб отримати додаткову довідку й підтримку в цій статті.

**Я хочу використовувати Microsoft Graph, але не знаєте, з чого почати**

- [Огляд Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Огляд ідентифікації та керування доступом у Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Початок роботи зі створення програм Microsoft Graph](https://docs.microsoft.com/graph/)
- **Провідник Microsoft Graph** – перевірка API Microsoft Graph у клієнті або демонстраційному клієнті

**Я хочу використовувати Microsoft Graph, але вона підтримує API 1,0 для каталогу, яку мені потрібно?**

Microsoft Graph – це рекомендований API для каталогів, посвідчень та керування доступом. Однак, між можливими в лазуровому графіку і Microsoft Graph ще кілька прогалин. Перегляньте наведені нижче статті, які висвітлюють актуальні відмінності для надання допомоги у виборі:

- [Відмінності між типами ресурсів у Azure AD Graph і Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Відмінності між майновими ОГОЛОШЕННЯМИ та Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Відмінності між методами Azure AD і Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Під час виклику API не працює – де можна виконувати додаткові перевірки?**

**Microsoft Graph Explorer** – перевірка API Microsoft Graph у клієнті чи демонстраційному клієнті, а також перегляньте **Приклади запитів** у провіднику Microsoft Graph.

**Моя програма дуже низька, а також її обмежується. Які удосконалення можна зробити?**

Залежно від сценарію, у вашому розпорядженні є різні варіанти, щоб зробити програму більш продуктивнішою, а в деяких випадках менше схильні до задуми служби (коли ви робите дуже багато дзвінків).

- [Практичні поради з роботи з Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Запити на дозування](https://docs.microsoft.com/graph/json-batching)
- [Відстеження змін через Дельта-запит](https://docs.microsoft.com/graph/delta-query-overview)
- [Отримання сповіщень про зміни через вебгачки](https://docs.microsoft.com/graph/webhooks)
- [Вказівки щодо дроселювання](https://docs.microsoft.com/graph/throttling)

**Де можна знайти додаткові відомості про помилки та відомі проблеми?**

- [Відомості про помилки під час відгуку Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Відомі проблеми з Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Де можна перевірити стан доступності та підключення служби?**

Доступність служб і зв'язок із базовими службами, які можна отримати за допомогою Microsoft Graph, може вплинути на загальну доступність та продуктивність Microsoft Graph.

- У розділі справність служби "Azure Active Directory" Перевірте стан служби **безпеки + посвідчення** , що відображається на [сторінці "стан Лазур](https://azure.microsoft.com/status/)".
- Для служб Office, які беруть участь у програмі Microsoft Graph, перевірте стан служб, перелічених на [приладній дошці служби Office](https://portal.office.com/adminportal/home#/servicehealth).

Помилки авторизації Microsoft Graph можуть бути результатом кількох різних проблем, більшість з яких створює помилку 401 або 403. Наприклад, наведені нижче дії можуть призвести до помилок авторизації:

- Неправильні [потоки отримання маркерів доступу](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Неналежне налаштування [областей дозволів](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Відсутність [дозволу](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_Кінець підтримки бібліотеки автентифікації Azure Active Directory (ADAL) і API Azure AD Graph (AAD Graph)_* _

_ * Починаючи з 30 червня 2020 * *, ми більше не будемо додавати нові функції до РЕКЛАМНОГО графіку ADAL і Azure. Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.

**Починаючи з 30 червня 2022** р., ми ЗАВЕРШУВАТИМЕМО підтримку рекламного графіку Adal і Azure, які більше не зможуть надавати технічну підтримку та оновлення системи безпеки.

Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не *отримають жодної технічної підтримки або оновлень системи безпеки*.

Програми, що використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки, що відображається в Лазурне AD.

**Міграція ADAL**

Ми радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.

Якщо ви використовуєте програми Microsoft, відомо, що корпорація Майкрософт перебуває в процесі перенесення своїх програм до служби MSAL на термін до кінця підтримки, гарантуючи, що вони будуть користуватися поточною безпекою та удосконаленнями функцій MSAL.

1. [Запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Дізнайтеся, як перенести програми платформами](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Якщо вам потрібна допомога з розумінням, які програми використовують ADAL, радимо переглянути всі вихідні коди програми, а також, якщо це можливо, охопити будь-які постачальники або постачальники програм. Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому осередку.

**Перенесення AAD Graph**

Для програм, які використовують Azure AD Graph, дотримуйтеся вказівок, щоб [перенести застосунки AZURE AD Graph до Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Контрольний список перенесення для початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. На порталі реєстрації Azure показано, які програми використовують AAD Graph. Радимо переглянути вихідний код усіх своїх програм і, за необхідності, зв’язатися з будь-якими незалежними постачальниками програмного забезпечення або постачальниками програм. Служба підтримки Microsoft також може надати вам список усіх видів використання AAD Graph у вашому клієнті.
3. Щоб отримати доступ до даних у програмі Microsoft Graph, користувач або адміністратор має надати йому відповідні дозволи за допомогою процесу згоди. [Довідник із дозволів Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) містить список дозволів, пов'язаних із кожним основним набором API Microsoft Graph. Це також дає вказівки про те, як використовувати дозволи.
