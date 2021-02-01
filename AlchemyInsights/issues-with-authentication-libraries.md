---
title: Проблеми з бібліотеками автентифікації
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063703"
---
# <a name="issues-with-authentication-libraries"></a>Проблеми з бібліотеками автентифікації

1. [Бібліотеки автентифікації в програмі Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) , що підтримуються, і сумісні з ними, а бібліотеки з підтримкою Microsoft.
2. Бібліотека автентифікації Microsoft (MSAL) підтримує кілька [потоків автентифікації](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) для використання в різних сценаріях програм.
3. Щоб автентифікувати та придбати маркери, ви ініціалізаєте нову загальнодоступну або конфіденційну клієнтську програму в коді. Під час ініціалізації програми клієнта в бібліотеці автентифікації Microsoft (MSAL) можна настроїти кілька параметрів конфігурації. Докладні відомості наведено в статті [Параметри конфігурації застосунку](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Кінець підтримки бібліотеки автентифікації в Azure Active Directory (ADAL) та API Azure AD Graph (AAD Graph)**

**Починаючи з 30 червня 2020** р., ми більше не додаватимуть нові функції на графіку adal і AZURE AD. Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.

**Починаючи з 30 червня 2022** р., ми ЗАВЕРШУВАТИМЕМО підтримку рекламного графіку Adal і Azure, які більше не зможуть надавати технічну підтримку та оновлення системи безпеки.

Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не *отримають жодної технічної підтримки або оновлень системи безпеки*.

Програми, що використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки, що відображається в Лазурне AD.

**Міграція ADAL**

Ми радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.

Якщо ви використовуєте програми Microsoft, відомо, що корпорація Майкрософт перебуває в процесі перенесення своїх програм до служби MSAL на термін до кінця підтримки, гарантуючи, що вони отримають вигоду від поточної системи безпеки й вдосконалення функцій MSAL.

Докладні відомості:

1. [Запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Дізнайтеся, як перенести програми платформами](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Якщо вам потрібна допомога з розумінням, які програми використовують ADAL, радимо переглянути всі вихідні коди програми, а також, якщо це можливо, охопити будь-які постачальники або постачальники програм. Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому клієнті.

**Перенесення AAD Graph**

Для програм, які використовують Azure AD Graph, дотримуйтеся вказівок, щоб [перенести застосунки AZURE AD Graph до Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Наш контрольний список перенесення містить точку початку роботи.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. На порталі реєстрації Azure показано, які програми використовують AAD Graph. Радимо переглянути вихідний код усіх своїх програм і, за необхідності, зв’язатися з будь-якими незалежними постачальниками програмного забезпечення або постачальниками програм. Служба підтримки Microsoft також може надати вам список усіх видів використання AAD Graph у вашому клієнті.
3. Щоб отримати доступ до даних у програмі Microsoft Graph, користувач або адміністратор має надати йому відповідні дозволи за допомогою процесу згоди. [Довідник із дозволів Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference) містить список дозволів, пов'язаних із кожним основним набором API Microsoft Graph. Це також дає вказівки про те, як використовувати дозволи.
