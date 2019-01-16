---
title: Перетворення поштової скриньки користувача на спільну поштову скриньку?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28319751"
---
<span data-ttu-id="8bc29-p101">Можна тільки перетворювати поштової скриньки користувача для спільної поштової скриньки, якщо користувач має ліцензію Exchange. Після того, як поштової скриньки перетворюється, він буде продовжувати відображатися у списку активних користувачів, оскільки цей список включає в себе спільні поштові скриньки. Однак, перетвореного поштової скриньки також з'являться у списку спільної поштової скриньки.</span><span class="sxs-lookup"><span data-stu-id="8bc29-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="8bc29-p102">Якщо ви спробуєте перетворити поштової скриньки у консолі адміністратора Exchange і перетворення здійснено неуспішно, очистьте кеш веб-переглядача та файли cookie і повторіть спробу. Якщо він все ще працює, спробуйте перетворити поштової скриньки Exchange Management Shell, запустивши таку команду:</span><span class="sxs-lookup"><span data-stu-id="8bc29-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="8bc29-107">Більш поштової скриньки перетворення детальна інформація доступна в [перетворити користувача поштову скриньку для спільної поштової скриньки](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="8bc29-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
