---
title: Архівна поштова скринька майже заповнена
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046773"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Архівна поштова скринька майже заповнена

Якщо користувач отримає попередження; **Архівна поштова скринька** майже заповнена або потрібно збільшити розмір архівної поштової скриньки, ось кілька порад:

1. Якщо користувачу призначено план Exchange Online (план 1), оновіть систему до Exchange Online (план **2),** щоб збільшити розмір із 50 ГБ до 100 ГБ.
1. Якщо користувачу вже призначено один із таких варіантів: Exchange Online (план **2)** або Exchange Online (план 1) з додатковим компонентом архівація Exchange Online), виконайте наведені нижче дії, щоб активувати автоматичне розгортання архівування.
 
    1. [Підключення, щоб Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Запустіть для користувача такий командлет:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Щоб підтвердити, що для користувача ввімкнуто цю функцію, запустіть такий командлет:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Докладні відомості див. в такому:

- [Активація необмеженої архівації – довідка для адміністраторів Microsoft 365 відповідності | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online обмеження – описи служб | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Оновіть свій бізнес-план до іншого | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

