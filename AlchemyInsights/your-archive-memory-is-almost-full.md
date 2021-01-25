---
title: Поштову скриньку архіву майже заповнено
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974668"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Поштову скриньку архіву майже заповнено

Якщо користувач отримує попередження; **Поштова скринька архіву майже повна** або потрібно збільшити розмір поштової скриньки архіву, ось кілька порад:

1. Якщо для користувача призначено план Exchange Online 1, оновіть ліцензію на службу **Exchange Online Plan 2** , щоб збільшити розмір від 50 ГБ до 100 ГБ.
1. Якщо користувач уже призначається один із таких пунктів: **Exchange Online Plan 2** або Exchange Online Plan 1 із надбудовою архівування Exchange Online, виконайте наведені нижче дії, щоб активувати автоматичне розширення архівації:.
 
    1. [Підключіться до Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Виконайте такі дії чином для користувача:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Виконайте наведені нижче чином, щоб підтвердити, що його активовано для користувача.  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Докладні відомості наведено в статті:

- [ Активувати необмежену архівацію – Довідка для адміністратора – відповідність вимогам Microsoft 365 | Документи Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Обмеження Exchange Online – описи служб | Документи Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Оновлення до іншої бізнес-плану | Документи Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

