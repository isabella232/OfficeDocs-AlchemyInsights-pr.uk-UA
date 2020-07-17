---
title: Повідомлення, надіслані до Microsoft 365 групи не отримують всі члени
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051521"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Повідомлення, надіслані до групи Microsoft 365, не отримуються всіма членами

Переконайтеся, що всі учасники групи підписалися на отримання повідомлень електронної пошти. Дивіться [дотримуйтесь групи в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Щоб перевірити стан повідомлення користувачів, які підписалися на групу повідомлень електронної пошти, виконайте таку команду, на [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`