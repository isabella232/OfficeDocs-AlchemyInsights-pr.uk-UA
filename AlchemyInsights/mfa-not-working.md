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
# <a name="issues-with-azure-mfa"></a>Проблеми з Azure MFA
Якщо користувачам не вдається ввійти за допомогою багатофакторної автентифікації (MFA), потрібно виконати кілька речей.

1. Можливо, відповідного користувача заблоковано на порталі Azure Active Directory. У такому разі спроби автентифікації для певного користувача буде автоматично відхилено. [Щоб розблокувати їх, виконайте кроки, описані в цій статті.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Якщо розблокування користувача не допомогло, або його не заблоковано, можна спробувати скинути параметри MFA для користувача, і він повторить процес реєстрації ще раз. [Виконайте кроки, описані в цій статті.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Якщо ви вперше ввімкнете багатофагову автентифікацію, а користувачі не можуть ввійти в клієнти, що не надійшли в браузери, як-от Outlook, Skype тощо, можливо, в передплаті O365 не активовано ADAL (бібліотека автентифікації Active Directory). У цьому випадку потрібно підключитися до Exchange Online PowerShell і запустити цей командлет:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*