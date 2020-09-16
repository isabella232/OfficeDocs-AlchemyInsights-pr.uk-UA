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
# <a name="issues-with-azure-mfa"></a>Проблеми з "Блакитний МЗС"
Щоб перевірити, чи користувачі не можуть ввійти в систему за допомогою багатофакторної автентифікації (МЗС), можна скористатися кількома способами.

1. Користувач може заблокувати на порталі Azure Active Directory. Якщо це так, спроби автентифікації для певного користувача буде автоматично відмовлено. [Виконайте кроки, описані в цій статті, щоб розблокувати їх.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Якщо розблокувати користувача не допомогло або користувач не заблокував, ви можете спробувати скинути програму "МЗС" для користувача, і вони знову будуть проходити процес реєстрації. [Виконайте кроки, описані в цій статті.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Якщо ви вперше активували МЗС, а ваші користувачі не зможуть ввійти в клієнти, які не є браузерами, наприклад Outlook, Skype і т. д., можливо, у вашій передплаті O365 не активовано функцію ADAL (бібліотека автентифікації Active Directory). У цьому випадку вам доведеться підключитися до Exchange Online PowerShell і запустити цей командлет:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $TRUE*