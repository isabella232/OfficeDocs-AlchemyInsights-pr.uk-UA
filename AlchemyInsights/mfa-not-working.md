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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768858"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="cdec4-102">Проблеми з МЗС Azure</span><span class="sxs-lookup"><span data-stu-id="cdec4-102">Issues with Azure MFA</span></span>
<span data-ttu-id="cdec4-103">Є кілька речей, щоб перевірити, якщо користувачі не можуть увійти в систему за допомогою багатофакторної аутентифікації (МЗС)</span><span class="sxs-lookup"><span data-stu-id="cdec4-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="cdec4-104">Відповідного користувача може бути заблоковано на порталі Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cdec4-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="cdec4-105">Якщо це так, спроби автентифікації для конкретного користувача будуть автоматично відхилені.</span><span class="sxs-lookup"><span data-stu-id="cdec4-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="cdec4-106">Будь ласка, виконайте дії, описані в цій статті, щоб розблокувати їх.</span><span class="sxs-lookup"><span data-stu-id="cdec4-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="cdec4-107">Якщо розблокування користувача не допомогло, або користувач не заблоковано, можна спробувати скинути МЗС для користувача, і вони будуть проходити процес зарахування знову.</span><span class="sxs-lookup"><span data-stu-id="cdec4-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="cdec4-108">Будь ласка, дотримуйтесь інструкцій, наведених у цій статті.</span><span class="sxs-lookup"><span data-stu-id="cdec4-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="cdec4-109">Якщо це перший раз, коли ви ввімкнули МЗС і ваші користувачі не в змозі увійти в систему не браузерів, таких як Outlook, Skype і т. д., можливо, ADAL (Active Directory автентифікації бібліотека) не включений на вашу передплату O365.</span><span class="sxs-lookup"><span data-stu-id="cdec4-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="cdec4-110">У цьому випадку вам потрібно буде підключитися до Exchange Online PowerShell і запустити цю команду:  *Set-Організаціїconfig-OAuth2ClientProfileEnabled: $TRUE*</span><span class="sxs-lookup"><span data-stu-id="cdec4-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>