---
title: Під час аналітики desktop Analytics під час перевірення маркера доступу сталася помилка
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813709"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="713ca-102">Під час підключення до Desktop Analytics сталася помилка під час перевірки маркера доступу</span><span class="sxs-lookup"><span data-stu-id="713ca-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="713ca-103">Зазвичай ця помилка виникає після завершення терміну дії маркера автентифікації.</span><span class="sxs-lookup"><span data-stu-id="713ca-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="713ca-104">Зазвичай після оновлення сторінки оновлюється маркер.</span><span class="sxs-lookup"><span data-stu-id="713ca-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="713ca-105">Однак ця проблема може виникати, якщо до облікового запису застосовуються будь-які політики умовного доступу, застосовані до борту Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="713ca-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="713ca-106">Ви можете переглянути журнали входу в Azure AD на порталі Azure, щоб дізнатися, чи не вдається ввійти в обліковий запис, який використовується для підключення до Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="713ca-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="713ca-107">Докладні відомості про умовний доступ див. в [цьому документі.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="713ca-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>