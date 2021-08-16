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
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028025"
---
# <a name="issues-with-authentication-libraries"></a>Проблеми з бібліотеками автентифікації

1. [платформа ідентичностей Microsoft бібліотек автентифікації](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) перелічено бібліотеки клієнтів і середнього програмного забезпечення, сумісні з Microsoft.
2. Бібліотека Microsoft Authentication Library (MSAL) підтримує кілька потоків автентифікації для використання в різних сценаріях програм. [](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows)
3. Щоб автентифікувати та отримати маркери, потрібно ініціалізувати нову загальнодоступну або конфіденційну клієнтську програму в коді. Якщо клієнт ініціалізовано в бібліотеці Microsoft Authentication Library (MSAL), можна задали кілька параметрів конфігурації. Докладні відомості див. в [статтях Параметри конфігурації програми.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Припинення підтримки бібліотек Azure Active Directory автентифікації (ADAL) і Azure AD Graph API (AAD Graph)**

**З 30 червня 2020** р. ми більше не додаватимемо нові функції до ADAL і Azure AD Graph. Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.

**З 30 червня 2022** року ми завершимо підтримку ADAL і Azure AD Graph і більше не надаватимемо технічну підтримку або оновлення системи безпеки.

Програми, які використовують ADAL у наявних версіях ОС, і надалі працюватиме після цього, але не отримуватимете *технічної підтримки або оновлень системи безпеки.*

Програми, які використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки Azure AD Graph.

**Перенесення ADAL**

Ми радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.

Якщо ви використовуєте програми Microsoft, зверніть увагу, що корпорація Майкрософт зараз переносить свої програми до служби MSAL до крайніх термінів припинення підтримки, забезпечивши їм постійну безпеку та вдосконалення функцій MSAL.

Докладні відомості:

1. [Запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Дізнайтеся, як перенести програми платформами](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Якщо вам потрібна допомога з розумінням того, які програми використовують ADAL, радимо переглянути вихідний код усіх програм і, за потреби, зв'язатися з інтернет-провайдерами або постачальниками програм. Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому осередку.

**Перенесення AAD Graph**

Для програм, які використовують Azure AD Graph, дотримуйтеся наших вказівок, щоб [перенести програми Azure AD Graph до microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Наш контрольний список перенесення забезпечує початок роботи.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. На порталі реєстрації Azure показано, які програми використовують AAD Graph. Радимо переглянути вихідний код усіх своїх програм і, за необхідності, зв’язатися з будь-якими незалежними постачальниками програмного забезпечення або постачальниками програм. Крім того, служба підтримки Microsoft може надати список усіх Graph AAD у вашому клієнтів.
3. Щоб програма отримла доступ до даних у Graph Microsoft, користувач або адміністратор повинен надати їй відповідні дозволи в процесі згоди. У [посиланні Graph дозволів Microsoft](https://docs.microsoft.com/graph/permissions-reference) на перелічено дозволи, пов'язані з кожним основним набором API-Graph Microsoft. Тут також наведено інструкції з використання дозволів.
