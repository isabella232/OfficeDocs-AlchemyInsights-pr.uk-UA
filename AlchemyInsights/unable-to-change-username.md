---
title: Не вдається змінити ім'я користувача
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440294"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="882d7-102">Не вдається змінити ім'я користувача</span><span class="sxs-lookup"><span data-stu-id="882d7-102">Unable to change UserName</span></span>

<span data-ttu-id="882d7-103">У деяких випадках UPN (ім'я користувача) зміни не поширюються на хмарі.</span><span class="sxs-lookup"><span data-stu-id="882d7-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="882d7-104">Ви можете отримати помилки верифікації на порталі Office 365 або не можете змінити ім'я користувача або адресу електронної пошти.</span><span class="sxs-lookup"><span data-stu-id="882d7-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="882d7-105">Щоб вирішити цю проблему, вручну встановити ім'я користувача за допомогою цієї команди PowerShell.</span><span class="sxs-lookup"><span data-stu-id="882d7-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="882d7-106">**Приклад: перейменування користувача**</span><span class="sxs-lookup"><span data-stu-id="882d7-106">**Example: Rename a user**</span></span>

<span data-ttu-id="882d7-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="882d7-107">PowerShellCopy</span></span>

<span data-ttu-id="882d7-108">PS C: \> Set-MsolUserPrincipalName-користуваяназва "davidc@contoso.com"-новимназва "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="882d7-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="882d7-109">Ця команда перейменовує davidc@contoso.com на davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="882d7-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="882d7-110">Щоб отримати додаткові відомості, [див.](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)</span><span class="sxs-lookup"><span data-stu-id="882d7-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>