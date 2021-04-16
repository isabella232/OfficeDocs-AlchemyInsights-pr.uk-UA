---
title: Проблеми з MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810505"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="b2a45-102">Проблеми з Azure MFA</span><span class="sxs-lookup"><span data-stu-id="b2a45-102">Issues with Azure MFA</span></span>
<span data-ttu-id="b2a45-103">Якщо користувачам не вдається ввійти за допомогою багатофакторної автентифікації (MFA), потрібно виконати кілька речей.</span><span class="sxs-lookup"><span data-stu-id="b2a45-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="b2a45-104">Можливо, відповідного користувача заблоковано на порталі Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b2a45-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="b2a45-105">У такому разі спроби автентифікації для певного користувача буде автоматично відхилено.</span><span class="sxs-lookup"><span data-stu-id="b2a45-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="b2a45-106">Щоб розблокувати їх, виконайте кроки, описані в цій статті.</span><span class="sxs-lookup"><span data-stu-id="b2a45-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="b2a45-107">Якщо розблокування користувача не допомогло, або його не заблоковано, можна спробувати скинути параметри MFA для користувача, і він повторить процес реєстрації ще раз.</span><span class="sxs-lookup"><span data-stu-id="b2a45-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="b2a45-108">Виконайте кроки, описані в цій статті.</span><span class="sxs-lookup"><span data-stu-id="b2a45-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="b2a45-109">Якщо ви вперше ввімкнете багатофагову автентифікацію, а користувачі не можуть ввійти в клієнти, що не надійшли в браузери, як-от Outlook, Skype тощо, можливо, в передплаті O365 не активовано ADAL (бібліотека автентифікації Active Directory).</span><span class="sxs-lookup"><span data-stu-id="b2a45-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="b2a45-110">У цьому випадку потрібно підключитися до Exchange Online PowerShell і запустити цей командлет:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="b2a45-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>