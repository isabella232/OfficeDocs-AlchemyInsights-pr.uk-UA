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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098623"
---
# <a name="issues-with-azure-mfa"></a>Проблеми з Azure MFA
Якщо користувачам не вдається ввійти за допомогою багатофакторної автентифікації (MFA), потрібно виконати кілька речей.

1. Відповідного користувача може бути заблоковано на Azure Active Directory порталі. У такому разі спроби автентифікації для певного користувача буде автоматично відхилено. [Щоб розблокувати їх, виконайте кроки, описані в цій статті.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Якщо розблокування користувача не допомогло, або його не заблоковано, можна спробувати скинути параметри MFA для користувача, і він повторить процес реєстрації ще раз. [Виконайте кроки, описані в цій статті.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Якщо ви вперше ввімкнете багатофагову автентифікацію, а користувачі не можуть входити в клієнти, не з яких не підтримуються браузери, як-от Outlook, Skype тощо, можливо, ADAL (бібліотека автентифікації Active Directory) не активовано в передплаті O365. У цьому випадку потрібно підключитися до Exchange Online PowerShell і виконати цей командлет: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*