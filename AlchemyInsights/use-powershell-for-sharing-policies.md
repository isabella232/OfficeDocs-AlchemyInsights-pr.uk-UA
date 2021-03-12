---
title: Скористайтеся Windows PowerShell для Політик спільного доступу та Зв’язків організації
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: cd1d34e4dae474e61c799ca9234b2f18c718f27b
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709487"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Скористайтеся Windows PowerShell для Політик спільного доступу та Зв’язків організації


Для Зв’язків організації перегляньте докладні відомості про синтаксис і параметри для : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ТА [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Щоб створити політику спільного доступу, скористайтеся [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Щоб [застосувати політику спільного доступу до поштової скриньки або користувача](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes), потрібно використовувати з новою політикою поєднання [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) і [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox). Щоб [змінити, вимкнути або видалити політику спільного доступу](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy), потрібно використовувати [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) і [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Щоб мати повне розуміння цієї теми, див.:**

[Надання спільного доступу в Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)