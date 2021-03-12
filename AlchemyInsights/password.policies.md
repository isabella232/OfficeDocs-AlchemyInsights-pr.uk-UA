---
title: Політики паролів
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 826e266d08aa68c0d4213d8058a0244f404fe965
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747057"
---
# <a name="password-policies"></a><span data-ttu-id="f3659-102">Політики паролів</span><span class="sxs-lookup"><span data-stu-id="f3659-102">Password policies</span></span>

<span data-ttu-id="f3659-103">**У мене виникли проблеми з політикою паролів для користувача**</span><span class="sxs-lookup"><span data-stu-id="f3659-103">**I'm having problems with the password policy for a user**</span></span>

- <span data-ttu-id="f3659-104">Політика паролів для користувача залежить від того, чи є користувач хмарним або локальною.</span><span class="sxs-lookup"><span data-stu-id="f3659-104">The password policy for a user depends on whether the user is cloud only or on-premises.</span></span>
- <span data-ttu-id="f3659-105">Хмарні лише користувачі мають вибрати пароль, який відповідає вимогам цієї статті: [політики паролів, які застосовуватимуться лише до облікових записів користувачів у хмарі](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts) .</span><span class="sxs-lookup"><span data-stu-id="f3659-105">Cloud only users must choose a password that meets the requirements in this article: [Password policies that only apply to cloud user accounts](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)</span></span>
- <span data-ttu-id="f3659-106">Локальні користувачі мають вибрати пароль, який відповідає локальним вимогам.</span><span class="sxs-lookup"><span data-stu-id="f3659-106">On-premises users must choose a password that meets the on-premises requirements.</span></span> <span data-ttu-id="f3659-107">Якщо локальний користувач не може встановити пароль, перевірте свої локальні вимоги.</span><span class="sxs-lookup"><span data-stu-id="f3659-107">If an on-premises user is unable to set their password, check your on-premises requirements.</span></span>

<span data-ttu-id="f3659-108">**Я не знаю, як установлювати або перевіряти політики терміну дії паролів**</span><span class="sxs-lookup"><span data-stu-id="f3659-108">**I don't know how to set or check password expiration policies**</span></span>

- <span data-ttu-id="f3659-109">Ви можете встановити та перевірити політику терміну дії для хмарних користувачів у клієнті за допомогою PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f3659-109">You can set and check the expiration policy for cloud users in your tenant by using PowerShell.</span></span> <span data-ttu-id="f3659-110">Виконайте вказівки, описані в цій статті: [Установлення або перевірка політик паролів за допомогою PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span><span class="sxs-lookup"><span data-stu-id="f3659-110">Follow the instructions in this article: [Set or check the password policies by using PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)</span></span>
- <span data-ttu-id="f3659-111">Політика терміну дії пароля для локальних користувачів встановлюється в локальній службі AD.</span><span class="sxs-lookup"><span data-stu-id="f3659-111">The password expiration policy for on-premises users is set in your on-premises AD.</span></span>

<span data-ttu-id="f3659-112">**Інші корисні посилання:**</span><span class="sxs-lookup"><span data-stu-id="f3659-112">**Other Helpful links:**</span></span>
- [<span data-ttu-id="f3659-113">Початок роботи з Скидмою пароля</span><span class="sxs-lookup"><span data-stu-id="f3659-113">Getting Started with Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [<span data-ttu-id="f3659-114">Виправлення неполадок із Скидленням пароля адміністратора</span><span class="sxs-lookup"><span data-stu-id="f3659-114">Troubleshoot Administrator-initiated Password Reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
