---
title: Проблеми, що розвиваються програми з API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975022"
---
# <a name="issues-developing-applications-with-apis"></a>Проблеми, що розвиваються програми з API

Щоб почати використовувати API для роботи з програмою Azure Active Directory, ознайомтеся з посібником із короткого посібника з використання служби Azure [AD GRAPH API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , або перегляньте [довідкову документацію API Azure AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Кінець підтримки бібліотеки автентифікації в Azure Active Directory (ADAL) та API Azure AD Graph (AAD Graph)**

**Починаючи з 30 червня 2020** р., ми більше не додаватимуть нові функції на графіку adal і AZURE AD. Ми продовжимо надавати технічну підтримку та оновлення системи безпеки, але більше не зможете надавати оновлення функцій.

**Починаючи з 30 червня 2022** р., ми ЗАВЕРШУВАТИМЕМО підтримку рекламного графіку Adal і Azure, які більше не зможуть надавати технічну підтримку та оновлення системи безпеки.

Програми, які використовують ADAL на наявних версіях ОС, продовжуватимуть працювати після цього часу, але не отримають жодної технічної підтримки або оновлень системи безпеки.

Програми, що використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки, що відображається в Лазурне AD.

**Міграція ADAL**

Радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.

Якщо ви використовуєте програми Microsoft, відомо, що корпорація Майкрософт перебуває в процесі перенесення своїх програм до служби MSAL на термін до кінця підтримки, гарантуючи, що вони будуть користуватися поточною безпекою та удосконаленнями функцій MSAL.

1. [Прочитайте запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Дізнайтеся, як перенести програми на платформу для кожної платформи](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Якщо вам потрібна допомога з розумінням, які програми використовують ADAL, радимо переглянути всі вихідні коди програми, а також, якщо це можливо, охопити будь-які постачальники або постачальники програм. Служба підтримки Microsoft також може надати вам список всіх програм, які не належать до Microsoft ADAL у вашому клієнті.

**Міграція AAD графа**

Для програм, які використовують Azure AD Graph, дотримуйтеся вказівок, щоб перенести [застосунки AZURE AD Graph до Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Наш контрольний список перенесення містить точку початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. На порталі реєстрації в програмі Azure App показано, які програми використовують AAD Graph. Радимо переглянути всі вихідні коди програм, а також, якщо це можливо, охопити будь-які постачальники ПЗ або провайдери програм. Служба підтримки Microsoft також може надати вам список усіх видів використання AAD Graph у вашому клієнті.
1. Щоб отримати доступ до даних у програмі Microsoft Graph, користувач або адміністратор має надати йому відповідні дозволи за допомогою процесу згоди. [Довідник із дозволів Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) містить список дозволів, пов'язаних із кожним основним набором API Microsoft Graph. Це також дає вказівки про те, як використовувати дозволи.
