---
title: Змінення надійних вимог до паролів
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818489"
---
# <a name="change-strong-password-requirement"></a>Змінення надійних вимог до паролів

За замовчуванням корпорація Майкрософт вимагає використовувати надійні паролі.

За допомогою PowerShell можна вимкнути надійні паролі для певних користувачів за допомогою таких команд:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Щоб вимкнути надійні паролі для всіх користувачів, використовуйте:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Докладні відомості про політику паролів](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Підключення до Microsoft 365 за допомогою PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Докладні відомості про команди PowerShell MsolUser](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
