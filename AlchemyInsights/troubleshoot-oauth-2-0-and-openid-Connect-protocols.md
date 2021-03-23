---
title: Усунення несправностей із протоколами OAuth 2,0 і OpenID
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037694"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>Усунення несправностей із протоколами OAuth 2,0 і OpenID

Щоб вирішити проблеми з OAuth 2,0 і "Вконтакте", виконайте наведені нижче Рекомендовані дії.

Зверніться до наведених нижче статей, пов'язаних із конфігурацією та виправлення неполадок із протоколами OAuth 2,0 і OpenID Connect:

- [Служба ідентифікації Microsoft і OAuth 2,0 код авторизації](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – у цій статті розповідається про те, як програмувати безпосередньо з **потоку грантів коду (pkce)** у вашій програмі, використовуючи будь-яку мову.
- У цій статті описано, як безпосередньо з **потоком клієнтів** у вашій програмі описується програма [ідентифікації клієнта Microsoft і обліковий потік облікових даних клієнтів OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) .
- [Облікові дані власника ресурсу служби ідентифікації Microsoft і OAuth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) – у цій статті описано, як програмувати безпосередньо на **потік ropc** у вашій програмі.
    - Платформа ідентифікації Microsoft підтримує лише ROPC для користувачів Azure AD, а не для особистих облікових записів. Це означає, що ви повинні використовувати кінцеву точку клієнта **( https://login.microsoftonline.com/{TenantId_or_Name})** або кінцеву точку **організації** ).
    - Особисті облікові записи, які запрошують на Azure-клієнт AD, не можуть використовувати ROPC.
    - Облікові записи, які не мають паролів, не можуть входити через ROPC. Щоб скористатися цим сценарієм, радимо використовувати інший потік для програми.
    - Якщо користувачам потрібно використовувати [багатофакторну автентифікацію (МЗС)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) для входу в програму, їх буде заблоковано.
    - Функція ROPC не підтримується в сценаріях [гібридної Федерації ідентифікації](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) (наприклад, AZURE AD і adfs, які використовуються для автентифікації локальних облікових записів). Якщо користувачі повністю перенаправляються на локальну постачальника посвідчень, то Azure AD не може перевірити ім'я користувача та пароль для цього постачальника посвідчень. Однак, підтримка [автентифікації](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) за допомогою програми ropc.
    - Виняток для гібридного сценарію Федерації ідентифікації має бути таке: політика пошуку вдома за допомогою **AllowCloudPasswordValidation** , яка має значення **True** , дасть змогу виконати потік для роботи з федеративними користувачами, коли локальний пароль синхронізується з хмарою. Додаткові відомості можна знайти в статті [Увімкнення автентифікації на прямих ПК для використання в попередніх версіях програми для роботи з користувачами](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Платформа ідентифікації Microsoft і OAuth 2,0 від імені-потоку](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) – у цій статті розповідається про те, як програмувати безпосередньо від імені в програмі **(OBO) потоку** .
- [Платформа ідентифікації Microsoft і протокол HTTPS Connect](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – у цій статті описано, як реалізувати протокол HTTPS для підключення незалежно від мови, а також Дізнайтеся, як надсилати та отримувати повідомлення http без використання бібліотек із відкритим вихідним кодом Microsoft.

**Маркери доступу**

[Маркери доступу до платформи Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) : Дізнайтеся, як ваш API може перевіряти та використовувати скарги в маркер доступу. Усі документи в цій статті, за винятком випадків, коли вказано, застосовуються лише до маркерів, виданих для API, які ви зареєстрували. Він не застосовується до маркерів, виданих для API, які належать до корпорації Майкрософт, і не можуть використовувати маркери, щоб перевірити, як платформа ідентифікації корпорації Майкрософт видає маркери для створеного API.

**Конфігурація застосунку**

[ПЕРЕСПРЯМУВАННЯ URI (відповідь URL-адреси)](https://docs.microsoft.com/azure/active-directory/develop/reply-url) – Дізнайтеся, як настроїти URI переадресації (відповідь URL-адреси). Редирект або відповідь URL-адреса – це розташування, у якому сервер авторизації надсилає користувачу, коли програма успішно авторизована, і надав код авторизації або маркер доступу. Сервер авторизації надсилає код або маркер до URI переспрямування; тому важливо зареєструвати правильне розташування як частину процесу реєстрації програми.

**Підготовка програм**

[Навчальний посібник: розробка та планування підготовки до кінцевої точки SCIM](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) – у цій статті описано, як створити кінцеву точку SCIM та інтегрувати її за допомогою служби підготовки aad.


