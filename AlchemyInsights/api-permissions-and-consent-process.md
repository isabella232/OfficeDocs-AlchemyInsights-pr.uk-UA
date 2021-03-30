---
title: Дозволи API та процес згоди
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405445"
---
# <a name="api-permissions-and-consent-process"></a>Дозволи API та процес згоди

Щоб програма отримла доступ до даних у Microsoft Graph, користувач або адміністратор повинен надати їй відповідні дозволи в процесі згоди. [Microsoft Graph permissions reference lists](https://docs.microsoft.com/graph/permissions-reference) the permissions associated with each major set of Microsoft Graph API. Тут також наведено інструкції з використання дозволів.

**Настроювання або оновлення основного номера служби**

- [Створення об'єкта-служби. У](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) цій статті описано, як створити об'єкт servicePrincipal.
- Створення [основного ім'я](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) служби & Azure AD на порталі. У цій статті описано, як створити нову програму й основне ім'я служби Azure Active Directory (Azure AD), яку можна використовувати з елементом керування доступом на основі ролей.
- [Принципи програм &](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) служби в Azure AD. У цій статті описано реєстрацію програм, об'єкти програм і основні імена служб в Azure Active Directory: їхнє призначення, а також те, як вони пов'язані між собою.

**Додавання або оновлення реєстрації програм і надання згоди адміністратора**

- [Створіть реєстрацію програми.](https://docs.microsoft.com/graph/api/application-post-applications) У цій статті описано, як створити об'єкт програми.
- [Оновлення реєстрації програми – дозволи API.](https://docs.microsoft.com/graph/api/application-update) У цій статті описано, як оновити властивості об'єкта програми.
- [Надайте згоду](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) адміністратора. Щоб отримати згоду адміністратора та надати згоду в цілому, адміністратор має явно надати згоду.
- [RBAC (бета-система).](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) Контейнер керування ролями для уніфікованих визначень ролей і призначень ролей для постачальників Microsoft 365 RBAC, який підтримує кілька основних ролей і кількох областей в одному призначенні ролей. Цей тип ресурсу *відрізняється від типу ресурсу rbacApplication.* Microsoft Intune – приклад такого постачальника RBAC. Призначення ролей в Intune може мати масив основних значень і масив груп областей. **Це в бета-програмі, тобто вона ще на стадіях розробки та не рекомендується для використання в виробництво.**
