---
title: Проблеми з розробкою програм
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974763"
---
# <a name="issues-developing-applications"></a>Проблеми з розробкою програм

Щоб усунути найпоширеніші проблеми під час створення веб-програм "блакитні активні каталоги (AD)", ознайомтеся з такими статтями:

- [Я бачу проблеми з входом в програму лише за допомогою браузера Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Я не знаю, як змінити параметри терміну дії маркера для моєї програми](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Я заплутався про те, як працює згода на використання програми](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Я не знаю, як надати дозволи для моєї програми](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Я не можу розібратися в різниці між делегованих і дозволами на використання програми](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Кінець підтримки бібліотеки автентифікації в Azure Active Directory (ADAL) та API AZURE AD Graph (AAD Graph)** _

- Починаючи з 30 червня 2020, ми більше не додаватимуть нові функції в бібліотеці автентифікації Azure Active Directory (ADAL) і Azure AD Graph API (AAD Graph). Ми продовжимо надавати технічну підтримку та оновлення системи безпеки, але більше не зможете надавати оновлення функцій.

- Починаючи з 30 червня 2022 р., ми завершуємо підтримку на графіку ADAL і AAD, і більше не зможете надавати технічну підтримку та оновлення системи безпеки. У результаті цієї умови наведені нижче наслідки наведені нижче дії.

    - Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не отримають жодної технічної підтримки або оновлень системи безпеки.

    - Програми, що використовують AAD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки AAD графа

_ *Adal перенесення**

Якщо ви використовуєте програми Microsoft, радимо оновити бібліотеку автентифікації Microsoft (MSAL), яка містить найновіші функції та оновлення системи безпеки. Ця рекомендація в контексті Microsoft ініціює процес перенесення своїх програм до MSAL до кінцевого терміну підтримки. 

Міграція корпорацією Майкрософт своїх програм для MSAL гарантує, що програми отримують вигоду від поточної безпеки та удосконалень функцій MSAL.

1. [Читайте запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Відомості про перенесення програм на основі платформи](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Якщо вам потрібна допомога в розумінні того, що ваші програми використовують ADAL, радимо переглянути всі вихідні коди програм і, за потреби, відповідати всім незалежним постачальникам програмного забезпечення (постачальникам ПЗ) або постачальникам програм. Служба підтримки Microsoft також може надати вам список всіх програм, які не належать до Microsoft ADAL у вашому клієнті.

**Міграція AAD графа**

Для програм, що використовують AAD Graph, дотримуйтеся вказівок, щоб перенести програми AAD Graph до Microsoft Graph:

1. [Наш контрольний список перенесення містить точку початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. На порталі реєстрації в програмі Azure App показано, які програми використовують AAD Graph. Радимо переглянути всі вихідні коди програм і, за необхідності, охопити будь-які незалежні постачальники програмного забезпечення (незалежні постачальники ПЗ) або постачальники програм. Служба підтримки Microsoft також може надати вам інформацію про використання графіків у вашому клієнті.







