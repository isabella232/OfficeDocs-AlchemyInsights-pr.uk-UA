---
title: Проблеми з посиланнями та URL-адресами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321928"
---
# <a name="issues-with-links-and-urls"></a>Проблеми з посиланнями та URL-адресами

Універсальний ідентифікатор ресурсу (URI) переспрямування чи URL-адреси відповіді (обидва вирази взаємозамінні) – це URL-адреси, які використовуються платформою ідентичностей Microsoft, щоб повертати маркери, які запитала програма. Відомості про ці URL-адреси див. в таких статтях:

- [Потоки автентифікації та сценарії програм](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – відомості про URI переспрямування на сторінці **Реєстрація програми** для кожного сценарію.
- [Обмеження URI переспрямування та URL-адрес відповіді](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Не знаю, як зареєструвати правильний URI переспрямування або URL-адресу відповіді для своєї програми**

Якщо ви входите за допомогою програми, яку розробляєте, і відображається діалогове вікно входу **AADSTS50011: URL-адреса відповіді, указана в запиті, не відповідає налаштованим для програми URL-адресам відповіді<your app ID>**, потрібно додати до реєстрації програми URI переспрямування, який ваш код використав у запиті маркера до платформи ідентичностей Microsoft.

Щоб додати URL-адресу відповіді, перейдіть на вкладку **Автентифікація** на сторінці **Реєстрації програми** порталу Microsoft Azure і додайте запис у розділі **URI переспрямування**. Значення, яке потрібно ввести, залежить від типу програми, яку ви будуєте, як описано нижче.

- Для односторінкових програм і веб-програм URL-адреса відповіді – це URL-адреса в програмі. Див. [Реєстрації односторінкової програми](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) або [Зареєструйте веб-програму на порталі Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Для класичних програм потрібне значення залежить від такого:
    - платформа (MacOS відрізняється від Windows або Linux)
    - спосіб придбання маркера (інтерактивно, з потоком коду пристрою, за допомогою вбудованої автентифікації Windows [IWA] або з іменем користувача і паролем).
    Докладні відомості див. в статті [Класичні програми – реєстрація програм – URІ переспрямування](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- Для мобільних програм URI переспрямування залежить від такого:
    - платформа (iOS/Android/UWP)
    - відомості, використані для створення програми, наприклад ідентифікатор пакета в iOS або ім’я пакета та геш підпису в Android. Вам допоможе реєстрація програми на порталі Microsoft Azure. Докладні відомості див. в статті [Конфігурації платформи та URI переспрямування](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

**Примітка.** Для веб-інтерфейсів API та деяких беззвучних способів отримання маркерів (IWA та ім'я користувача та пароль) ідентифікатор URI не потребує переспрямування.

**У мене розгорнута веб-програма, і коли я її тестую, з’являється повідомлення про невідповідність URL-адреси відповіді**

Додайте URI переспрямування для всіх розташувань, у яких розгортаєте веб-програму. Докладні відомості див. в статті [Реєстрація веб-програми за допомогою порталу Microsoft Azure](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

**Примітка.** Додайте URI переспрямування для розташування відразу після розгортання програми в цьому розташуванні.

**Не вдається зареєструвати достатню кількість URL-адрес відповіді**

Ви – ISV і маєте один або кілька URI переспрямування для кожного клієнта. Потрібно перенести з ADAL/Azure AD v 1.0 до MSAL або платформи ідентичностей Microsoft, але досягнуто [максимальної кількості URI переспрямування](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Щоб вирішити цю проблему, [додайте URI переспрямування до принципалів служби](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals), які відповідають кожному з ваших клієнтів.
