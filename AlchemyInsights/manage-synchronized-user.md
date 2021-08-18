---
title: Керування синхронізованим користувачем
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: bfa66492397adfd121fd3c9ddb2c190394cbc9a771a3e2c2db656ad438e404f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114805"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Не вдається вказати основну адресу електронної пошти, змінити атрибути користувача або видалити синхронізованого користувача

Якщо синхронізацію служби каталогів увімкнуто для вашого середовища, деякі атрибути користувача або об'єкта не можна змінити за допомогою Центр адміністрування Microsoft 365.

Щоб повністю керувати синхронізованими користувачами та їхніми атрибутами, використовуйте локальну консоль керування користувачами Active Directory та групами (adsiedit.msc).  

Крім того, ви можете змінити окремих користувачів або атрибути для синхронізних користувачів за допомогою PowerShell, як показано в наведених нижче прикладах.

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
