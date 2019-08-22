---
title: Проблеми з МЗС
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545207"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="f7578-102">Проблеми з МЗС</span><span class="sxs-lookup"><span data-stu-id="f7578-102">Issues with MFA</span></span>
<span data-ttu-id="f7578-103">Є кілька речей, щоб перевірити, якщо користувачі не можуть увійти, використовуючи багатофакторну автентифікацію (МЗС)</span><span class="sxs-lookup"><span data-stu-id="f7578-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="f7578-104">Уражені користувача може бути заблоковано Azure Active Directory на порталі.</span><span class="sxs-lookup"><span data-stu-id="f7578-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="f7578-105">Якщо це так, спроб автентифікації для цього конкретного користувача буде автоматично відмовлено.</span><span class="sxs-lookup"><span data-stu-id="f7578-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="f7578-106">Будь ласка, виконайте дії, описані в цій статті, щоб розблокувати їх.</span><span class="sxs-lookup"><span data-stu-id="f7578-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="f7578-107">Якщо розблокування користувач не допомагає, або користувач не блокується спробуйте скинути МЗС для користувача, і вони будуть проходити Реєстрація процес знову.</span><span class="sxs-lookup"><span data-stu-id="f7578-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="f7578-108">Будь ласка, виконайте дії, описані в цій статті.</span><span class="sxs-lookup"><span data-stu-id="f7578-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="f7578-109">Якщо це перший раз із підтримкою МЗС і ваших користувачів, ти не дозволив вхід для клієнтів браузерів, таких як Outlook, Skype, і т. д, може бути ADAL (активних каталогів автентифікації бібліотека) не ввімкнуто O365 передплати.</span><span class="sxs-lookup"><span data-stu-id="f7578-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="f7578-110">У цьому випадку вам потрібно буде підключитися до Exchange Online Powershell та запуску цього командлета:  *набір-Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="f7578-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>