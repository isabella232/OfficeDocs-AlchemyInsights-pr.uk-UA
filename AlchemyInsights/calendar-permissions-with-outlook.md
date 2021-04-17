---
title: Дозволи календаря
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819929"
---
# <a name="calendar-permissions"></a>Дозволи календаря

Користувачі можуть змінювати власні дозволи календаря в інтернет-версії Outlook або інших клієнтах, але як адміністратор може також вивчати цю мету.  
Якщо за допомогою командлета Exchange PowerShell з'являться дозволи в календарі користувача, виконайте такі дії:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Докладні відомості див. в таких статтях:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Дозволи календаря використовуються для надання спільного доступу до календарів. Докладні відомості про надання спільного доступу до календаря Outlook див. в таких статтях:

- [Надання спільного доступу до календаря Outlook іншим користувачам](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Надання спільного доступу до календаря в інтернет-версії Outlook для бізнесу](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Виправлення неполадок із календарем. Дозвіл можна отримати за [допомогою помічника з підтримки й](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) відновлення.