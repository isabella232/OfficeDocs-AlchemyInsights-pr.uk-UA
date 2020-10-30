---
title: Змінення надійного вимоги для пароля
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
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804444"
---
# <a name="change-strong-password-requirement"></a>Змінення надійного вимоги для пароля

Корпорація Майкрософт вимагає надійних паролів за замовчуванням.

За допомогою PowerShell можна вимкнути надійні паролі для певних користувачів за допомогою цих команд:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Щоб вимкнути надійні паролі для всіх користувачів, використовуйте такі дії:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Додаткові відомості про політику паролів](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Підключення до Microsoft 365 за допомогою PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Додаткові відомості про команди PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
