---
title: Сталася помилка під час перевірки помилки маркера доступу під час настільних аналітику на основі програми-інтернату
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783572"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="8388a-102">Помилка під час перевірки помилки "Маркер доступу" під час настільних аналітики переходу</span><span class="sxs-lookup"><span data-stu-id="8388a-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="8388a-103">Ця помилка зазвичай спостерігається, коли термін дії маркера автентифікації завершується.</span><span class="sxs-lookup"><span data-stu-id="8388a-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="8388a-104">Зазвичай оновлення сторінки оновлює маркер.</span><span class="sxs-lookup"><span data-stu-id="8388a-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="8388a-105">Однак ця проблема може зберігатися, якщо в обліковому записі, що використовується для настільних комп'ютерів, застосовуються будь-які політики умовного доступу, застосовані до облікового запису.</span><span class="sxs-lookup"><span data-stu-id="8388a-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="8388a-106">Щоб дізнатися, чи є помилки входу для облікового запису, який використовується для настільних аналізування, можна переглянути в журналах лазуровий вхід на порталі Azure AD.</span><span class="sxs-lookup"><span data-stu-id="8388a-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="8388a-107">Щоб отримати докладні відомості про умовний доступ, перегляньте [план розгортання умовного доступу](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="8388a-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>