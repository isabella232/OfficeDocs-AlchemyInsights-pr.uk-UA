---
title: Секрет клієнта реєстрації програм або проблеми з сертифікатом
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
- "9004352"
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405328"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="18f8b-102">Секрет клієнта реєстрації програм або проблеми з сертифікатом</span><span class="sxs-lookup"><span data-stu-id="18f8b-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="18f8b-103">Завершення терміну дії секрету клієнта програм?</span><span class="sxs-lookup"><span data-stu-id="18f8b-103">Application client secret expiring?</span></span>

<span data-ttu-id="18f8b-104">Незалежно від способу створення зареєстрованої програми, стандартний процес реєстрації на порталі реєстрації програм або якщо в клієнті створено основне ім'я служби за допомогою згоди програми, потрібно створити новий секрет клієнта до завершення терміну дії поточної та оновленої в пов'язаному коді програм.</span><span class="sxs-lookup"><span data-stu-id="18f8b-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="18f8b-105">Максимальний період чинності – 2 роки.</span><span class="sxs-lookup"><span data-stu-id="18f8b-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="18f8b-106">Нагадуємо, що таємне значення має бути записано, оскільки воно більше не відображатиметься на сторінці Реєстрації програм на порталі.</span><span class="sxs-lookup"><span data-stu-id="18f8b-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="18f8b-107">Докладні відомості див. в [статті Короткий посібник:](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) реєстрація програми на платформі ідентичності Microsoft і Рекомендації щодо платформи [ідентичності Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="18f8b-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="18f8b-108">Докладні відомості див. в статті Створення програми Azure AD & основного ім'я служби на [порталі – платформі ідентичності Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="18f8b-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
