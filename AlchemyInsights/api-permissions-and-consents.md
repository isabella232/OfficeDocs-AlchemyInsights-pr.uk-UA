---
title: Дозволи для API та згоду
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974998"
---
# <a name="api-permissions-and-consent"></a>Дозволи для API та згоду

Програми, які інтегруються з ідентифікацією платформи Microsoft, наслідуємо модель авторизації, яка дає користувачам і адміністраторам змогу керувати тим, як можна отримати доступ до даних. На кінцевій точці платформи Microsoft ідентифікації оновлено відповідну модель авторизації. У цій статті описано, як програма має взаємодіяти з платформою ідентифікації Microsoft. [Дозволи та згода в кінцевій точці платформи Microsoft ідентифікації відповідно](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) до основних понять цієї моделі авторизації, зокрема областей, дозволів і згоди.

[Структура згоди «Лазурний» (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) дає змогу легко розробляти веб-програми з кількома клієнтськими та рідними клієнтами. Ці програми дають змогу ввійти за допомогою облікових записів користувачів із Неблакитного РЕКЛАМНОГО клієнта, який відрізняється від того, де буде зареєстрований застосунок. Вони також можуть отримати доступ до веб-API, наприклад API Microsoft Graph (щоб отримати доступ до Azure AD, Inune та Services в Microsoft 365) та інших API служб Microsoft Services, крім власного веб-API.

