---
title: Проблеми з розробленням програм за допомогою API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013481"
---
# <a name="issues-developing-applications-with-apis"></a>Проблеми з розробленням програм за допомогою API

Щоб почати використовувати інтерфейс API Azure Active Directory Graph, див. короткий посібник користувача [Azure AD Graph API](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) або перегляньте інтерактивну довідку з [API Azure AD Graph API.](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)

**Припинення підтримки бібліотек Azure Active Directory автентифікації (ADAL) і Azure AD Graph API (AAD Graph)**

**З 30 червня 2020** р. ми більше не додаватимемо нові функції до ADAL і Azure AD Graph. Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.

**З 30 червня 2022** року ми завершимо підтримку ADAL і Azure AD Graph і більше не надаватимемо технічну підтримку або оновлення системи безпеки.

Програми, які використовують ADAL у наявних версіях ОС, продовжуватимуть працювати, але не отримуватимуть технічної підтримки чи оновлень системи безпеки.

Програми, які використовують Azure AD Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки Azure AD Graph.

**Перенесення ADAL**

Ми радимо оновити [бібліотеку автентифікації Microsoft (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), яка містить найновіші функції та оновлення системи безпеки.

Якщо ви використовуєте програми Microsoft, зверніть увагу, що корпорація Майкрософт зараз переносить свої програми до служби MSAL до крайніх термінів припинення підтримки, забезпечивши їм постійну безпеку та вдосконалення функцій MSAL.

1. [Прочитайте запитання й відповіді про ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Дізнайтеся, як перенести програми на платформі.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Якщо вам потрібна допомога з розумінням того, які програми використовують ADAL, радимо переглянути вихідний код усіх програм і, за потреби, зв'язатися з інтернет-провайдерами або постачальниками програм. Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому осередку.

**Перенесення AAD Graph**

Для програм, які використовують Azure AD Graph, дотримуйтеся наших вказівок, щоб перенести [програми Azure AD Graph до microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Контрольний список перенесення для початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. На порталі реєстрації Azure показано, які програми використовують AAD Graph. Радимо переглянути вихідний код усіх своїх програм і, за необхідності, зв’язатися з будь-якими незалежними постачальниками програмного забезпечення або постачальниками програм. Крім того, служба підтримки Microsoft може надати список усіх Graph AAD у вашому клієнтів.
1. Щоб програма отримла доступ до даних у Graph Microsoft, користувач або адміністратор повинен надати їй відповідні дозволи в процесі згоди. У [посиланні Graph дозволів Microsoft](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) на перелічено дозволи, пов'язані з кожним основним набором API-Graph Microsoft. Тут також наведено інструкції з використання дозволів.
