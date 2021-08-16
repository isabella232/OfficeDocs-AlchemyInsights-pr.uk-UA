---
title: Увімкнення аудиту поштових скриньок
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
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058059"
---
# <a name="turn-on-mailbox-auditing"></a>Увімкнення аудиту поштових скриньок

Щоб увімкнути аудит поштових скриньок для одного користувача або всієї організації, запустіть ці командлети з Remote PowerShell:

- **Окремий** користувач: Set-Mailbox ідентичності "Яна Доу" -AuditEnabled $true
- **Організація:** Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true

Докладні відомості див. в [розділі Керування аудитом поштових скриньок.](https://go.microsoft.com/fwlink/?linkid=2103668)