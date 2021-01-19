---
title: Проблеми зі згоди адміністратора
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901516"
---
# <a name="admin-consent-issues"></a>Проблеми зі згоди адміністратора

1. Увімкнення [робочого циклу адміністратора](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , щоб користувачі могли запитувати схвалення адміністратора безпосередньо з екрана згоди.

1. Якщо ви або користувачі програми бачитимуть несподівані помилки під час процесу згоди, перегляньте цю статтю для виправлення неполадок: [неочікувана помилка під час виконання згоди на програму](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Дізнайтеся більше про [згоду адміністратора на платформі ідентифікації Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), як працює [запит на згоду](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) , і як [оцінити запит на отримання згоди адміністратора](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Програми, які інтегруються з ідентифікацією платформи Microsoft, наслідуємо модель авторизації, яка дає користувачам і адміністраторам змогу керувати тим, як можна отримати доступ до даних. На кінцевій точці платформи Microsoft Identity (модель авторизації) Оновлено відповідний компонент, і він змінює спосіб взаємодії програми з програмою ідентифікації Microsoft. Перегляньте [дозволи та згоду в кінцевій точці платформи Microsoft Identity](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) для огляду цієї моделі авторизації, зокрема областей, дозволів і згоди.