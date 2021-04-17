---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830603"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Працюєте з Оболонкою PowerShell або сценаріями в Sharepoint Online? Щоб отримати докладні відомості, перейдіть за посиланнями нижче.
- [Початок роботи з оболонкою керування SharePoint Online](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [Підключення до SPO PowerShell за допомогою багатофакторної автентифікації (MFA)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- Шаблони та практики [SharePoint (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) містить бібліотеку команд PowerShell, за допомогою яких можна виконувати складні дії з керування для SPO.

> [!NOTE]
> - Якщо виникають проблеми з підключенням до оболонки керування SPO, переконайтеся, [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) що ви оновили модуль до найновішої версії, і спробуйте повторно імпортувати його за допомогою *команди "Import-Module Microsoft.Online.SharePoint.PowerShell".*
> - Якщо ви намагаєтеся запустити сценарії об'єктної моделі на боці клієнта, на локальному комп'ютері має бути інстальовано пакет SDK для клієнтських компонентів [SharePoint Online.](https://www.microsoft.com/download/details.aspx?id=42038)
> - Якщо у вас виникають проблеми із виконанням сценаріїв з PowerShell, можливо, ви захочете запустити PowerShell як адміністратор і змінити [політику виконання.](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)