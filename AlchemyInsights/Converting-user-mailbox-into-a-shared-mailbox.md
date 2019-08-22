---
title: Перетворення поштової скриньки користувача на спільну поштову скриньку?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496456"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a>Перетворення спільної поштової скриньки користувача поштова скринька

Можна тільки перетворювати поштової скриньки користувача для спільної поштової скриньки, якщо користувач має ліцензію Exchange. Після того, як поштової скриньки перетворюється, він буде продовжувати відображатися у списку активних користувачів, оскільки цей список включає в себе спільні поштові скриньки. Однак, перетвореного поштової скриньки також з'являться у списку спільної поштової скриньки. 
  
Якщо ви спробуєте перетворити поштової скриньки у консолі адміністратора Exchange і перетворення здійснено неуспішно, очистьте кеш веб-переглядача та файли cookie і повторіть спробу. Якщо він все ще працює, спробуйте перетворити поштової скриньки Exchange Management Shell, запустивши таку команду:
  
```
Set-Mailbox -Type Shared
```

Більш поштової скриньки перетворення детальна інформація доступна в [перетворити користувача поштову скриньку для спільної поштової скриньки](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).
  
