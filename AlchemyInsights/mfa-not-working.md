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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250186"
---
# <a name="issues-with-mfa"></a>Проблеми з МЗС
Є кілька речей, щоб перевірити, якщо користувачі не можуть увійти, використовуючи багатофакторну автентифікацію (МЗС)

1. Уражені користувача може бути заблоковано Azure Active Directory на порталі. Якщо це так, спроб автентифікації для цього конкретного користувача буде автоматично відмовлено. [Будь ласка, виконайте дії, описані в цій статті, щоб розблокувати їх.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Якщо розблокування користувач не допомагає, або користувач не блокується спробуйте скинути МЗС для користувача, і вони будуть проходити Реєстрація процес знову. [Будь ласка, виконайте дії, описані в цій статті.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Якщо це перший раз із підтримкою МЗС і ваших користувачів, ти не дозволив вхід для клієнтів браузерів, таких як Outlook, Skype, і т. д, може бути ADAL (активних каталогів автентифікації бібліотека) не ввімкнуто O365 передплати. У цьому випадку вам потрібно буде підключитися до Exchange Online Powershell та запуску цього командлета:  *набір-Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*