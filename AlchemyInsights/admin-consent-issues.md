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
# <a name="admin-consent-issues"></a><span data-ttu-id="22c72-102">Проблеми зі згоди адміністратора</span><span class="sxs-lookup"><span data-stu-id="22c72-102">Admin consent issues</span></span>

1. <span data-ttu-id="22c72-103">Увімкнення [робочого циклу адміністратора](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , щоб користувачі могли запитувати схвалення адміністратора безпосередньо з екрана згоди.</span><span class="sxs-lookup"><span data-stu-id="22c72-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="22c72-104">Якщо ви або користувачі програми бачитимуть несподівані помилки під час процесу згоди, перегляньте цю статтю для виправлення неполадок: [неочікувана помилка під час виконання згоди на програму](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="22c72-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="22c72-105">Дізнайтеся більше про [згоду адміністратора на платформі ідентифікації Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), як працює [запит на згоду](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) , і як [оцінити запит на отримання згоди адміністратора](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="22c72-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="22c72-106">Програми, які інтегруються з ідентифікацією платформи Microsoft, наслідуємо модель авторизації, яка дає користувачам і адміністраторам змогу керувати тим, як можна отримати доступ до даних.</span><span class="sxs-lookup"><span data-stu-id="22c72-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="22c72-107">На кінцевій точці платформи Microsoft Identity (модель авторизації) Оновлено відповідний компонент, і він змінює спосіб взаємодії програми з програмою ідентифікації Microsoft.</span><span class="sxs-lookup"><span data-stu-id="22c72-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="22c72-108">Перегляньте [дозволи та згоду в кінцевій точці платформи Microsoft Identity](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) для огляду цієї моделі авторизації, зокрема областей, дозволів і згоди.</span><span class="sxs-lookup"><span data-stu-id="22c72-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>