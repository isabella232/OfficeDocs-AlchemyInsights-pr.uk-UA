---
title: Проблеми з розробленням програм
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013445"
---
# <a name="issues-developing-applications"></a>Проблеми з розробленням програм

Щоб усунути найпоширеніші проблеми під час Azure Active Directory (AD), див. такі статті:

- [Під час входу в програми за допомогою браузера Chrome виникають проблеми](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Я не знаю, як змінити стандартні значення часу життя маркерів для програми](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Я плутанина з отриманням згоди програми](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Я не знаю, як надати дозволи програмі](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Я не розумію різницю між уповноваженими дозволами та дозволами програми](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Припинення підтримки бібліотек Azure Active Directory автентифікації (ADAL) і Azure AD Graph API (AAD Graph)***

- З 30 червня 2020 року ми не додаватимемо нові функції до бібліотеки автентифікації Azure Active Directory (ADAL) і API Azure AD Graph (AAD Graph). Ми й надалі надаватимемо технічну підтримку та оновлення системи безпеки, але більше не надаватимемо оновлення функцій.

- З 30 червня 2022 року ми припинимо підтримку ADAL і AAD Graph і більше не надаватимемо технічну підтримку чи оновлення системи безпеки. У результаті цієї умови випливає такі наслідки:

    - Програми, які використовують ADAL у наявних версіях ОС, продовжуватимуть працювати, але не отримуватимуть технічної підтримки чи оновлень системи безпеки.

    - Програми, які використовують Graph після цього часу, можуть більше не отримувати відповіді від кінцевої точки AAD Graph.

**Перенесення ADAL**

Якщо ви використовуєте програми Microsoft, радимо оновитися до бібліотеки Microsoft Автентифікації (MSAL), яка містить найновіші функції та оновлення системи безпеки. Ця рекомендація полягає в тому, що корпорація Майкрософт ініціює процес перенесення програм до служби MSAL до крайніх термінів припинення підтримки. 

Корпорація Майкрософт зі своїх програм переносить їх до msAL, щоб забезпечити постійну безпеку та вдосконалення функцій MSAL для програм.

1. [Запитання й відповіді про ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Дізнайтеся, як перенести програми платформами](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Якщо вам потрібна допомога з розумінням того, які програми використовують ADAL, радимо переглянути весь вихідний код програм і, за потреби, зв'язатися з будь-яким незалежним постачальником програмного забезпечення (ISV) або постачальниками програм. Служба підтримки Microsoft також може надати список усіх сторонніх програм ADAL у вашому осередку.

**Перенесення AAD Graph**

У програмах, які використовують Graph AAD, дотримуйтеся цих інструкцій, щоб перенести програми AAD Graph до microsoft Graph:

1. [Контрольний список перенесення для початку роботи](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. На порталі реєстрації Azure показано, які програми використовують AAD Graph. Радимо переглянути всі вихідні коди програм і, за потреби, зв'язатися з ними з будь-яким незалежним постачальником програмного забезпечення (ISV) або постачальниками програм. Служба підтримки Microsoft також може надавати вам відомості про використання Graph AAD у вашому клієнтів.







