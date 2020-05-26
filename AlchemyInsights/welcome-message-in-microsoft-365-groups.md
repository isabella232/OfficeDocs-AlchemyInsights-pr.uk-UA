---
title: Привітальне повідомлення у групах Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358333"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Привітальне повідомлення у групах Microsoft 365

Нові користувачі, приєднання до Microsoft 365 групи буде отримувати вітальний повідомлення електронної пошти, якщо властивість "Unifiedfunfesmicrosofficrosoft"

Якщо ви хочете вимкнути привітальне повідомлення, скористайтеся такою командою [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) :

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
