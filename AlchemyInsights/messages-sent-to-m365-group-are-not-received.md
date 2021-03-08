---
title: Деякі учасники не отримали повідомлення, надіслані групі Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 080c060f5675065704c7209bd15e4cbb1236b8db
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480704"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Деякі учасники не отримали повідомлення, надіслані групі Microsoft 365

Переконайтеся, що всі учасники групи підписалися на електронні листи. Див. статтю [Підписка на групу в Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Щоб перевірити стан повідомлення для учасників, які підписалися на електронні листи групи, виконайте таку команду в [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Налаштуйте, щоб усі учасники групи отримували листи, надіслані групі Microsoft 365, у своїй папці "Вхідні", скориставшись такою командою EXO PowerShell:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Наприклад:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`