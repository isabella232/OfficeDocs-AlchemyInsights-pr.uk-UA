---
title: Зміна надійного пароля
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706582"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="33971-102">Зміна надійного пароля</span><span class="sxs-lookup"><span data-stu-id="33971-102">Change strong password requirement</span></span>

<span data-ttu-id="33971-103">За умовчанням корпорація Майкрософт вимагає надійних паролів.</span><span class="sxs-lookup"><span data-stu-id="33971-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="33971-104">За допомогою PowerShell можна вимкнути надійні паролі для певних користувачів за допомогою цієї команди:</span><span class="sxs-lookup"><span data-stu-id="33971-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="33971-105">*Набір-MsolUser – ім'я <UserPrincipalName> користувача – стронпасворсобов'язково $false*</span><span class="sxs-lookup"><span data-stu-id="33971-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="33971-106">Більш детальну інформацію про політику паролів</span><span class="sxs-lookup"><span data-stu-id="33971-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="33971-107">Як підключитися до Microsoft 365 з PowerShell</span><span class="sxs-lookup"><span data-stu-id="33971-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="33971-108">Додаткові відомості про команди PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="33971-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
