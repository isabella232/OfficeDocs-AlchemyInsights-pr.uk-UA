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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545207"
---
# <a name="issues-with-mfa"></a>Проблеми з МЗС
Є кілька речей, щоб перевірити, якщо користувачі не можуть увійти з використанням декількох факторів аутентифікації (МЗС)

1. Відповідного користувача може бути заблоковано на порталі Azure Active Directory. Якщо це так, спроби автентифікації для конкретного користувача будуть автоматично відхилені. [Будь ласка, виконайте дії, описані в цій статті, щоб розблокувати їх.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Якщо розблокування користувача не допомогло, або користувач не заблоковано, можна спробувати скинути МЗС для користувача, і вони будуть проходити процес зарахування знову. [Будь ласка, дотримуйтесь інструкцій, наведених у цій статті.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Якщо це перший раз, коли ви ввімкнули МЗС і ваші користувачі не в змозі увійти в систему не браузерів, таких як Outlook, Skype і т. д., можливо, ADAL (Active Directory автентифікації бібліотека) не включений на вашу передплату O365. У цьому випадку вам потрібно буде підключитися до Exchange Online PowerShell і запустити цю команду:  *Set-Організаціїconfig-OAuth2ClientProfileEnabled: $TRUE*