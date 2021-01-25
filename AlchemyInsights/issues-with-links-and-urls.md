---
title: Проблеми з посиланнями та URL-адресами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974758"
---
# <a name="issues-with-links-and-urls"></a>Проблеми з посиланнями та URL-адресами

Перенаправляти URI-URL-адреси (обидва вирази є взаємозамінними) – це URL-адреси, які використовуються в платформі ідентифікації програми Microsoft, щоб повернутися до відповідних маркерів. Щоб отримати відомості про ці URL-адреси, ознайомтеся з наведеними нижче статтями.

- [Перевірка потоків і сценарії застосунків](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) – відомості про перенаправлення URI на сторінці **реєстрації програми** для кожного сценарію.
- [Переспрямування та обмеження URL-адреси URI та відповіді](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**Я не знаю, як зареєструвати URL-адресу URI та відповіді для моєї програми**

Під час входу за допомогою програми, яку ви розробляєте, якщо діалогове вікно входу відображає **AADSTS50011: URL-адреса відповіді, указана в запиті, не відповідає URL-адресам відповідь, яку настроєно для програми <your app ID>**, потрібно додати до реєстрації програми, щоб переспрямувати URI, який код використовувався в запиті маркера до платформи Microsoft Identity.

Щоб додати URL-адресу відповіді, перейдіть на вкладку **автентифікація** на сторінці **реєстрації документів** на порталі Azure і додайте запис у розділі **перенаправлення URIs** . Ви ввели (веб-або мобільні або настільні). Значення, яке потрібно ввести, залежить від типу програми, яку ви створюєте, як описано нижче.

- URL-адреса для окремих сторінок і веб-програм має URL-адресу в програмі. Перегляд [документів на односторінкову реєстрацію](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) або [Реєстрація програми Web App за допомогою порталу Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- Для настільних програм значення, яке потрібно вибрати, залежить від:
    - платформа (MacOS відрізняється від Windows або Linux)
    - спосіб придбання маркера (в інтерактивному режимі з потоком коду пристрою з інтегрованою автентифікацією Windows [IWA] або з іменем користувача та паролем).
    Щоб отримати докладні відомості, перегляньте статтю [програми для настільних комп'ютерів: Реєстрація програми – переспрямування URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- У програмах для мобільних пристроїв, URI перенаправлення залежить від:
    - платформа (iOS/Android/UWP)
    - відомості, які використовуються для створення програми, наприклад ІДЕНТИФІКАТОР розшарування в iOS, а також назва пакета та геш підпису на платформі Android. Реєстрація програми «Лазурний портал» стане вам у нагоді. Докладні відомості наведено в статті [Конфігурація платформи та перенаправлення URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).

> [!NOTE]
> Веб-інтерфейси API та деякі мовчазні способи придбання маркерів (IWA та ім'я користувача та пароль) не вимагають переспрямування URI.

**Я розгорнута веб-застосунок і під час тестування розгорнутої програми з'являється повідомлення про невідповідність URL-адреси**

Додавання переспрямування URIs для всіх розташувань, у яких ви розгортаєте веб-програму. Додаткові відомості наведено в статті [Реєстрація програми Web App за допомогою порталу Azure Portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).

> [!NOTE]
> Після розгортання програми в цьому розташуванні можна додати до розташування URI переспрямування.

**Не вдається зареєструвати достатньо URL-адреси відповідей**

Ви є в службі ISV і маєте один або кілька перенаправляти URI для кожного клієнта. Потрібно перенести з ADAL/Azure AD v 1.0 на платформу ідентифікації Microsoft, і ви натиснете [максимальну кількість перенаправлення URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris). Щоб вирішити цю проблему, [додайте до принципалів служби](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) , які відповідають кожному зі своїх клієнтів.
