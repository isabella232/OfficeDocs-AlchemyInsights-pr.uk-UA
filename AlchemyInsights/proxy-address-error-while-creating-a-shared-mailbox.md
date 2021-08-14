---
title: Помилка адреси проксі-сервера під час створення спільної поштової скриньки
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062929"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>Помилка адреси проксі-сервера під час створення поштової скриньки або іншого об'єкта з підтримкою електронної пошти

Якщо під час спроби створити об'єкт із підтримкою електронної пошти (поштову скриньку, спільну поштову скриньку тощо) з'явилось повідомлення про помилку "Адреса проксі-сервера "SMTP:alias@domain.com" уже використовується...", вибрану адресу електронної пошти вже створено іншим об'єктом електронної пошти в організації.
  
Потрібно знайти користувача, групу, спільну поштову скриньку або спільну папку, яка містить цю адресу електронної пошти, і видалити її або змінити його адресу електронної пошти. Потім можна створити об'єкт із підтримкою електронної пошти з вивільненими адресами електронної пошти. Щоб знайти його, скористайтеся пошуком на домашній сторінці. Щоб знайти її, також можна Exchange Online виконати таку команду PowerShell:

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
Якщо не потрібно видаляти наявну адресу електронної пошти, виберіть нову адресу електронної пошти для нового об'єкта, який ви створюєте.
  