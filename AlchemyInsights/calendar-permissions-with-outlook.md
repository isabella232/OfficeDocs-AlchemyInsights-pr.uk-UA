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
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046125"
---
# <a name="calendar-permissions"></a>Дозволи календаря

Користувачі можуть змінювати власні дозволи календаря Outlook в Інтернеті або інших клієнтах, але адміністратору може знадобитися також дослідити цю можливість.  
Якщо Exchange командлет PowerShell, з'являться такі дозволи:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Докладні відомості див. в таких статтях:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Дозволи календаря використовуються для надання спільного доступу до календарів. Докладні відомості про надання спільного доступу до календаря Outlook див. в таких статтях:

- [Надання спільного доступу до календаря Outlook іншим користувачам](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Надання спільного доступу до календаря в інтернет-версія Outlook для бізнесу](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Виправлення неполадок із календарем. Дозвіл можна використовувати [Помічник із підтримки й відновлення](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) засобі.