---
title: Запити API Graph Microsoft
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923260"
---
# <a name="querying-the-microsoft-graph-api"></a>Запити API Graph Microsoft

Ця стаття також може застосовуватися до розробників, які продовжують використовувати Azure AD Graph API. Проте ми **наполегливо** рекомендуємо використовувати Microsoft Graph для всіх сценаріїв керування каталогами, ідентичностями та доступом.

**Проблеми з автентифікацією або авторизацією**

- Якщо програмі  не вдається отримати маркери для виклику в Microsoft Graph, виберіть елемент Проблема з отриманням маркера доступу **(автентифікації)** категорії Microsoft Graph, щоб отримати конкретнішу довідку та підтримку з цієї статті.
- Якщо під час виклику Microsoft Graph надходять помилки авторизації **401 або 403,** виберіть категорію Отримання помилки **(авторизації)** Microsoft Graph API, щоб отримати конкретнішу довідку та підтримку з цієї статті.

**Я хочу використовувати програму Microsoft Graph, але не знаєте, з чого почати**

Докладні відомості про microsoft Graph див. в статтях:

- [Огляд програми Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Огляд ідентичності та керування доступом у Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Початок роботи з програмами Microsoft Graph Microsoft](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – перевірка API Graph Microsoft у вашому клієнта або демонстрацією клієнта

**Я хочу використовувати Microsoft Graph але чи підтримується мені API каталогів v1.0?**

Microsoft Graph API для керування каталогами, ідентичноями та доступом. Проте між можливими розгалужень в Azure AD та Microsoft Graph і microsoft Graph. Перегляньте наведені нижче статті, у яких наведено найновіші відмінності, які можуть допомогти у виборі.

- [Відмінності між типами ресурсів між Azure AD Graph і Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Відмінності властивостей між Azure AD Graph і Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Відмінності між Azure AD та Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Коли я запитую *об'єкт* користувача, багато його властивостей відсутні**

`GET https://graph.microsoft.com/v1.0/users`Повертає лише 11 властивостей, оскільки Microsoft Graph автоматично вибирає стандартний набір *властивостей* користувача, які потрібно повернути. Якщо потрібні інші *властивості* користувача, скористайтеся $select, щоб вибрати властивості, потрібні для програми. Спочатку спробуйте зробити це в **Microsoft Graph Explorer.**

**Деякі значення властивостей користувача мають *Null-значення,* навіть якщо встановлено значення**

Найімовірніше, у програмі надано дозвіл *User.ReadBasic.All.* Це дасть змогу програмі читати обмежений набір властивостей користувача, повертаючи всі інші властивості як Null-значення, навіть якщо їх установлено раніше. Натомість спробуйте надати програмі *дозвіл User.Read.All.*

Докладні відомості див. в [статті Дозволи Graph Microsoft](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Виникли проблеми з використанням параметрів запиту OData для фільтрування даних у запитах**

Хоча microsoft Graph підтримує широкий діапазон параметрів запиту OData, багато з них не повністю підтримуються службами каталогів (ресурси, успадковані від *каталогуObject)* у програмі Microsoft Graph. Ті самі обмеження, що й в Azure AD, Graph на більшості випадків у Microsoft Graph:

1. **Не підтримується:**$count, $search або $filter *Null-значення* або *не Null-значення*
2. **Не підтримується:**$filter про певні властивості (див. розділи ресурсів про те, які властивості можна фільтрувати)
3. **Не підтримується:** дописання, фільтрування та сортування одночасно
4. **Не підтримується:** фільтрування за зв'язком. Наприклад, знайдіть усіх учасників інженерної групи у Великобританії.
5. **Часткова підтримка:**$orderby *користувач* (лише displayName і userPrincipalName) і *група*
6. Часткова **підтримка:**$filter (підтримується лише *eq,* *startswith* *,* або *,* і , і обмежена підтримка будь-якого), $expand (розширення зв'язків одного об'єкта повертає всі зв'язки, але розширення колекції зв'язків об'єктів обмежене)

Докладні відомості див. [в розділі Налаштування відповідей за допомогою параметрів запиту.](https://docs.microsoft.com/graph/query-parameters)

**Інтерфейс API, виклик якого я викликаю, не працює. Де можна виконати додаткові перевірки?**

**Microsoft Graph Explorer.** Тестуйте API-Graph Microsoft у вашому клієнта або демонстрацією клієнта,  а також перегляньте зразки запитів у Microsoft Graph Explorer.

**Якщо повернути запит на дані, схоже, що я поверную неповний набір даних**

Якщо ви запитуєте колекцію (наприклад, *користувачів),* корпорація Майкрософт Graph використовує обмеження на сторінки на сервері, тому результати завжди повертаються зі стандартним розміром сторінки. Завжди програма має розраховувати на сторінку колекцій, повернутих зі служби.

Докладні відомості:

- [Практичні Graph microsoft](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph data in your app](https://docs.microsoft.com/graph/paging)

**Моя програма задовга, і вона також дроселюється. Які вдосконалення можна вдосконалити?**

Залежно від сценарію у вашому розпорядженні існує багато різних варіантів, щоб програма стала більш функціональною, і в деяких випадках служба може зменшити дроселяці (у разі завеликої кількості викликів).

Докладніше про це див. в статтях:

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
