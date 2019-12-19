---
title: Сталася помилка під час перевірки маркер доступу до помилки робочого стола аналітика на посадку
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741304"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="5bb13-102">"Помилка перевірки маркер доступу" помилка під час робочого стола Analytics, публікування</span><span class="sxs-lookup"><span data-stu-id="5bb13-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="5bb13-103">Ця помилка зазвичай спостерігається після завершення терміну дії маркера автентифікації.</span><span class="sxs-lookup"><span data-stu-id="5bb13-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="5bb13-104">Зазвичай оновлення сторінки оновлюється маркером.</span><span class="sxs-lookup"><span data-stu-id="5bb13-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="5bb13-105">Проте ця проблема може зберігатися, якщо є будь-які політики умовного доступу, застосовані до облікового запису, що використовується для настільних Analytics.</span><span class="sxs-lookup"><span data-stu-id="5bb13-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="5bb13-106">Ви можете переглянути Azure AD входу в журналах Azure портал, щоб дізнатися, чи є будь-які неполадки входу для облікового запису, який використовується для публікування на робочому столі Analytics.</span><span class="sxs-lookup"><span data-stu-id="5bb13-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="5bb13-107">Щоб отримати додаткові відомості про умовний доступ, відвідайте [план розгортання умовного доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="5bb13-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>