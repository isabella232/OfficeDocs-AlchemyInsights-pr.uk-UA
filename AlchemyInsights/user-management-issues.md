---
title: Проблеми з керуванням користувачами
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037513"
---
# <a name="user-management-issues"></a>Проблеми з керуванням користувачами

**Що відбувається з поточним призначеним користувачам для програми, якщо не потрібно вимикати призначення користувача (для цього властивість не настроєно)?**

Вимкнення **призначення користувача** не впливає на зараз призначені користувачі. Вимкнення цієї властивості дасть змогу всім користувачам отримувати доступ до програми. Усі перелічені користувачі та користувачі, призначені групам у програмі, все ще будуть дійсними.

- Щоб обмежити програму певним набором користувачів, перегляньте статтю- [обмежити програму AZURE AD для набору користувачів – платформа ідентифікації Microsoft | Документи Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).
- Щоб призначити користувачам і групам, корпоративним програмам у лазурому Active Directory (Лазурний ОБ'ЯВІ), на основі блакитного порталу або за допомогою PowerShell, перегляньте статтю [керування призначенням користувача для програми в полі «Лазурний каталог](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)».
- Щоб делегувати дозволи на створення та керування програмами, ознайомтеся з [дозволами адміністратора Керування програмами--лазуровий AD | Документи Microsoft](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).
- **Приховайте певні корпоративні програми від користувачів** , виконайте наведені нижче дії, щоб приховати всі програми Microsoft 365 на панелі **myapps** . Програми все ще відображатимуться на порталі Office 365.

 1. Увійдіть на портал Azure як глобальний Адміністратор каталогу. 
 2. Виберіть пункт " **Лазурний**". 
 3. Виберіть елемент **користувачі**. 
 4. Виберіть елемент **Параметри користувача**. 
 5. У розділі **корпоративні програми** виберіть пункт Керування тим, **як кінцеві користувачі запускають та переглядають їхні програми**. 
 6. Щоб **користувачі могли переглядати лише програми office 365 на порталі office 365**, натисніть кнопку **так**. 
 7. Натисніть кнопку **Зберегти**. 
 8. Докладні відомості наведено в статті [приховання корпоративного застосунку з досвіду користувача в лазурое AD | Документи Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Якщо ви пропонуєте програмне забезпечення як застосунок-служба (SaaS) для багатьох організацій, ви можете налаштувати програму, щоб приймати вхід з будь-якого клієнта Azure Active Directory (Azure AD). Ця конфігурація називається "внесення багатоклієнтської програми". Користувачі в будь-якому клієнті Azure AD зможуть ввійти в програму після того, як ви погоджуєтеся використовувати свій обліковий запис у програмі. Докладні відомості наведено в статті [створення програм, які входу в Azure AD Users – платформа ідентифікації Microsoft | Документи Microsoft](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).

- **Як користувач може отримати доступ до програми, коли його призначено програмі?**

У кожній програмі у відповіді для корпоративної програми є посилання для користувачів, які можуть отримати доступ. Користувачі можуть також отримати доступ до програми за допомогою порталу **Myapps** у легкій формі.

- **Хочете знати, які програми та типи програм використовуються користувачами?**

Ви можете завантажити звіти про вхід за останні 30 днів із **portal.azure.com > Azure Active directory> Sigins> завантажити звіти**.

- Дізнайтеся, як [надати користувачу дозвіл на використання](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) клієнта, а також [настроїти умови згоди користувачів на програми](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).

- [Дізнайтеся, як](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) можна використовувати згоду та [керувати згодою для програм](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).


