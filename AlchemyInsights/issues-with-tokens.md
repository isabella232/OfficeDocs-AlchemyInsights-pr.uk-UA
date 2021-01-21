---
title: Проблеми з токени
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
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917213"
---
# <a name="issues-with-tokens"></a>Проблеми з токени

Щоб керувати проблемами, пов'язаними з токени, можна виконати наведені нижче дії.

1. Ви можете вказати термін дії маркера доступу, ІДЕНТИФІКАТОРА або САМБИ, виданого на платформі ідентифікації Microsoft. Ви можете встановити термін служби маркерів для всіх програм у вашій організації, для багатоклієнтської програми (мульти-організація) або для певної основної служби в організації. Щоб отримати докладніші відомості, ознайомтеся [з Настроювана маркером життя в платформі ідентифікації Microsoft (ознайомлювальну версію)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Маркери доступу дають клієнтам можливість безпечного виклику захищених веб-API та використовувати веб-API для виконання автентифікації та авторизації. За специфікацією OAuth, маркери Access – це непрозорі рядки без набору, який використовується для ідентифікації певних посвідчень (IDPs) за допомогою GUID-кодів, інші використовують зашифровані краплі. Платформа ідентифікації Microsoft використовує різні формати маркерів доступу, залежно від конфігурації API, що приймає маркер. Щоб дізнатися, як API можна перевіряти та використовувати скарги в маркер доступу, перегляньте [маркери доступу платформи Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Бібліотека автентифікації Microsoft (MSAL) підтримує кілька потоків автентифікації для використання в різних сценаріях програм. Щоб отримати докладніші відомості, ознайомтеся з [потоками автентифікації](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. У програмах, інстальованих на пристрої, щоб отримати доступ до захищених ресурсів, як-от веб-інтерфейси, можна використовувати Грант коду OAuth 2,0. Використовуючи 2,0 платформу ідентифікації корпорації Майкрософт, ви можете додавати до своїх мобільних і настільних програм доступ до служб входу та API. Дізнайтеся про те, як програма для роботи з протоколом у вашій програмі відображається на [платформі ідентифікації Microsoft і OAuth 2,0, а](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) також за допомогою будь-якої мови.
5. Функція OpenID Connect (OIDC) – це протокол автентифікації, вбудований у службу Auth 2,0, який можна використовувати для безпечного входу в програму. Під час використання кінцевої точки, що використовується в платформі ідентифікації сервера Microsoft, можна додати до програм вхід і API для входу. На [платформі ідентифікації Microsoft і в протоколі OpenID Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) показано, як це залежить від мови, і описується, як надсилати та отримувати повідомлення http без використання будь-яких бібліотек із відкритими вихідними кодами Microsoft.
    - Кінцева точка користувача – це частина стандарту OIDC, призначена для повернення тверджень про користувача, який автентифіковано. Щоб отримати докладніші відомості, ознайомтеся з [кінцевою точкою UserInfo платформи Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Виклик веб-API в веб-програмі за допомогою функції Azure AD і OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) приклад: створення веб-застосунку MVC, у якому використовується протокол Azure AD для входу за допомогою протоколу OpenID Connect, а також виклик веб-API в обліковому запису користувача за допомогою маркерів, отриманих за допомогою oauth 2,0. У цьому прикладі використовується програмне забезпечення проміжного програмного забезпечення OpenID і ADAL .net.
6. [Настройте програму, щоб викрити веб-API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – у цьому QuickStart можна зареєструвати веб-API за допомогою платформи ідентифікації Microsoft і викрити її в клієнтських програмах, додавши приклад області. Реєструючи веб-API та піддаючи його через області, можна надавати доступ до ресурсів для авторизованих користувачів і клієнтських програм, які мають доступ до API.
7. У надбудові B2C Active Directory (Azure AD B2C), дані паролів власника ресурсу (ROPC) – це стандартний потік автентифікації OAuth. У цьому потоці програма, яка також відома як сторона, що покладається, обмінюється дійсними обліковими даними для маркерів. Облікові дані містять ІДЕНТИФІКАТОР користувача та пароль. Повернуті маркери – це маркер ІДЕНТИФІКАТОРА, маркер доступу та маркер оновлення. Докладні відомості наведено в статті [Настроювання передавання облікових даних пароля власника ресурсу в службі Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

