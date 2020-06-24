---
title: Використання PowerShell для спільного використання політик і зв'язків організації
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862160"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Використання PowerShell для спільного використання політик і зв'язків організації


Для організації відносин перегляньте докладні відомості про синтаксис і параметр для: [Get-Федераціїінформація](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [нове організаціїзв'язок](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [настроїти організацію відносин](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) і [видалення](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship)організацій.

Щоб створити спільний доступ до політики, скористайтеся [SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Щоб [Застосувати політику спільного доступу до поштової скриньки або користувача](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) , потрібно скористатися комбінацією [Set-поштової скриньки](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) та [Get-поштової скриньки](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) з новоствореним політикою. Щоб [змінити, вимкнути або видалити політику спільного доступу,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) потрібно використовувати [параметр-sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) та [Видалити sharingpolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Для повного розуміння цієї теми, будь ласка, прочитайте:**

[Спільне використання в Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)