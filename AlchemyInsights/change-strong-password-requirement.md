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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="0fe99-102">Змінення надійного вимоги для пароля</span><span class="sxs-lookup"><span data-stu-id="0fe99-102">Change strong password requirement</span></span>

<span data-ttu-id="0fe99-103">Корпорація Майкрософт вимагає надійних паролів за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="0fe99-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="0fe99-104">За допомогою PowerShell можна вимкнути надійні паролі для певних користувачів за допомогою цих команд:</span><span class="sxs-lookup"><span data-stu-id="0fe99-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="0fe99-105">Щоб вимкнути надійні паролі для всіх користувачів, використовуйте такі дії:</span><span class="sxs-lookup"><span data-stu-id="0fe99-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="0fe99-106">Додаткові відомості про політику паролів</span><span class="sxs-lookup"><span data-stu-id="0fe99-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="0fe99-107">Підключення до Microsoft 365 за допомогою PowerShell</span><span class="sxs-lookup"><span data-stu-id="0fe99-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="0fe99-108">Додаткові відомості про команди PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="0fe99-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
