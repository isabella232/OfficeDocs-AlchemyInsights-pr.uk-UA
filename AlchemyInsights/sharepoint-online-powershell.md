---
title: Служба SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770860"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="8bc9a-102">Служба SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="8bc9a-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="8bc9a-103">Робота з PowerShell або скриптами в службі SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8bc9a-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="8bc9a-104">Перегляньте наведені нижче посилання, щоб отримати докладні відомості.</span><span class="sxs-lookup"><span data-stu-id="8bc9a-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="8bc9a-105">Початок роботи з оболонкою керування SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8bc9a-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="8bc9a-106">Підключення до програми SPO PowerShell із багатофакторною автентифікацією (МЗС)</span><span class="sxs-lookup"><span data-stu-id="8bc9a-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="8bc9a-107">[Шаблонами та практиками SharePoint (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) містить бібліотеку команд PowerShell, що дає змогу виконувати складні управлінські дії в напрямку SPO.</span><span class="sxs-lookup"><span data-stu-id="8bc9a-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="8bc9a-108">Якщо у вас виникли проблеми з підключенням оболонки керування за допомогою SPO, переконайтеся, що ви оновили останню версію та спробували [повторно імпортувати модуль](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) за допомогою *"Імпорт-модуль Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="8bc9a-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="8bc9a-109">Якщо ви намагаєтеся запустити сценарії для об'єктної моделі на боці клієнта, на локальному комп'ютері має бути інстальовано [компонент клієнта SharePoint Online](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="8bc9a-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="8bc9a-110">Якщо у вас виникли проблеми із сценаріями PowerShell, можливо, ви захочете запустити PowerShell як адміністратор і змінити [політику виконання](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="8bc9a-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>