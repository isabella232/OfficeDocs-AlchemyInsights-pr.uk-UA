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
ms.openlocfilehash: d888f4a208ccbc6f54469f5e1eb88f9f4197e5c9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47681893"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="55015-102">Змінення надійного вимоги для пароля</span><span class="sxs-lookup"><span data-stu-id="55015-102">Change strong password requirement</span></span>

<span data-ttu-id="55015-103">Корпорація Майкрософт вимагає надійних паролів за замовчуванням.</span><span class="sxs-lookup"><span data-stu-id="55015-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="55015-104">За допомогою PowerShell можна вимкнути надійні паролі для певних користувачів за допомогою цієї команди:</span><span class="sxs-lookup"><span data-stu-id="55015-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="55015-105">*Set-MsolUser – UserPrincipalName <UserPrincipalName> – необхідна $false*</span><span class="sxs-lookup"><span data-stu-id="55015-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="55015-106">Додаткові відомості про політику паролів</span><span class="sxs-lookup"><span data-stu-id="55015-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="55015-107">Підключення до Microsoft 365 за допомогою PowerShell</span><span class="sxs-lookup"><span data-stu-id="55015-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="55015-108">Додаткові відомості про команди PowerShell MsolUser</span><span class="sxs-lookup"><span data-stu-id="55015-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
