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
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545207"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="1af6a-102">Проблеми з МЗС</span><span class="sxs-lookup"><span data-stu-id="1af6a-102">Issues with MFA</span></span>
<span data-ttu-id="1af6a-103">Є кілька речей, щоб перевірити, якщо користувачі не можуть увійти з використанням декількох факторів аутентифікації (МЗС)</span><span class="sxs-lookup"><span data-stu-id="1af6a-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="1af6a-104">Відповідного користувача може бути заблоковано на порталі Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="1af6a-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="1af6a-105">Якщо це так, спроби автентифікації для конкретного користувача будуть автоматично відхилені.</span><span class="sxs-lookup"><span data-stu-id="1af6a-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="1af6a-106">Будь ласка, виконайте дії, описані в цій статті, щоб розблокувати їх.</span><span class="sxs-lookup"><span data-stu-id="1af6a-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="1af6a-107">Якщо розблокування користувача не допомогло, або користувач не заблоковано, можна спробувати скинути МЗС для користувача, і вони будуть проходити процес зарахування знову.</span><span class="sxs-lookup"><span data-stu-id="1af6a-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="1af6a-108">Будь ласка, дотримуйтесь інструкцій, наведених у цій статті.</span><span class="sxs-lookup"><span data-stu-id="1af6a-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="1af6a-109">Якщо це перший раз, коли ви ввімкнули МЗС і ваші користувачі не в змозі увійти в систему не браузерів, таких як Outlook, Skype і т. д., можливо, ADAL (Active Directory автентифікації бібліотека) не включений на вашу передплату O365.</span><span class="sxs-lookup"><span data-stu-id="1af6a-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="1af6a-110">У цьому випадку вам потрібно буде підключитися до Exchange Online PowerShell і запустити цю команду:  *Set-Організаціїconfig-OAuth2ClientProfileEnabled: $TRUE*</span><span class="sxs-lookup"><span data-stu-id="1af6a-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>