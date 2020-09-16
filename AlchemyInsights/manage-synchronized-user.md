---
title: Керування синхронізованим користувачем
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 53c188f6c6ab93bcc6f87d95717dc0d24d492bb7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47777698"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Не вдається встановити основну адресу електронної пошти, змінити атрибути користувача або видалити або видалити синхронізований користувач

Якщо для вашого середовища ввімкнуто синхронізацію служби каталогів, деякі атрибути користувача або об'єкта не можна змінити за допомогою Центру адміністрування Microsoft 365.

Щоб повністю керувати синхронізованими користувачами та усіма їхніми атрибутами, використовуйте локальну консоль керування користувачами та групами Active Directory (adsiedit. msc).  

Крім того, можна змінити окремі користувачі або атрибути для синхронізованих користувачів за допомогою PowerShell, як показано в таких поширених прикладах: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
