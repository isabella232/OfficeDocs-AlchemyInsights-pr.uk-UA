---
title: Увімкнення аудиту поштової скриньки
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483548"
---
# <a name="turn-on-mailbox-auditing"></a>Увімкнення аудиту поштової скриньки

Щоб увімкнути аудит поштової скриньки для одного користувача або всієї організації, запустіть наведені нижче командлети з віддаленого PowerShell:

- **Єдиний користувач**: Set-Mailbox-ідентичність "Джейн Dow" – AuditEnabled $True
- **Організація**: Get-Mailbox-ResultSize Unlimited-Filter {Reseientype(дані)-еквалайзер "usermailbox"} | Set-Mailbox-AuditEnabled $true

Докладні відомості наведено в статті [керування аудиторською поштовою скринькою](https://go.microsoft.com/fwlink/?linkid=2103668).