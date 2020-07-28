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
# <a name="unable-to-change-username"></a>Не вдається змінити ім'я користувача

У деяких випадках UPN (ім'я користувача) зміни не поширюються на хмарі. Ви можете отримати помилки верифікації на порталі Office 365 або не можете змінити ім'я користувача або адресу електронної пошти. Щоб вирішити цю проблему, вручну встановити ім'я користувача за допомогою цієї команди PowerShell.

**Приклад: перейменування користувача**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName-користуваяназва "davidc@contoso.com"-новимназва "davidchew@contoso.com"

Ця команда перейменовує davidc@contoso.com на davidchew@contoso.com.

Щоб отримати додаткові відомості, [див.](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)