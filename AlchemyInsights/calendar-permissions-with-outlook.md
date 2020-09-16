---
title: Дозволи календаря
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748814"
---
# <a name="calendar-permissions"></a>Дозволи календаря

Користувачі можуть змінювати власні дозволи календаря в Інтернет-версії Outlook або інших клієнтах, але як адміністратор може знадобитися також дослідити.  
За допомогою командлета Exchange PowerShell відобразиться дозвіл на календар користувача.

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Щоб переглянути додаткові відомості, ознайомтеся з такими відомостями:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Дозволи календаря використовуються в поданні "спільний доступ до календарів", щоб переглянути докладні відомості про надання спільного доступу до календаря Outlook, ознайомтеся з наведеними нижче статтями.

- [Надання спільного доступу до календаря Outlook іншим користувачам](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Надання спільного доступу до календаря в Інтернет-версії Outlook для бізнесу](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Щоб виправити неполадки календаря, ви можете використовувати засіб [помічник із підтримки та відновлення](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .