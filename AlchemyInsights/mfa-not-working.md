---
title: Проблеми з МЗС
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755152"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="20a22-102">Проблеми з "Блакитний МЗС"</span><span class="sxs-lookup"><span data-stu-id="20a22-102">Issues with Azure MFA</span></span>
<span data-ttu-id="20a22-103">Щоб перевірити, чи користувачі не можуть ввійти в систему за допомогою багатофакторної автентифікації (МЗС), можна скористатися кількома способами.</span><span class="sxs-lookup"><span data-stu-id="20a22-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="20a22-104">Користувач може заблокувати на порталі Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="20a22-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="20a22-105">Якщо це так, спроби автентифікації для певного користувача буде автоматично відмовлено.</span><span class="sxs-lookup"><span data-stu-id="20a22-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="20a22-106">Виконайте кроки, описані в цій статті, щоб розблокувати їх.</span><span class="sxs-lookup"><span data-stu-id="20a22-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="20a22-107">Якщо розблокувати користувача не допомогло або користувач не заблокував, ви можете спробувати скинути програму "МЗС" для користувача, і вони знову будуть проходити процес реєстрації.</span><span class="sxs-lookup"><span data-stu-id="20a22-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="20a22-108">Виконайте кроки, описані в цій статті.</span><span class="sxs-lookup"><span data-stu-id="20a22-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="20a22-109">Якщо ви вперше активували МЗС, а ваші користувачі не зможуть ввійти в клієнти, які не є браузерами, наприклад Outlook, Skype і т. д., можливо, у вашій передплаті O365 не активовано функцію ADAL (бібліотека автентифікації Active Directory).</span><span class="sxs-lookup"><span data-stu-id="20a22-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="20a22-110">У цьому випадку вам доведеться підключитися до Exchange Online PowerShell і запустити цей командлет:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*</span><span class="sxs-lookup"><span data-stu-id="20a22-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>