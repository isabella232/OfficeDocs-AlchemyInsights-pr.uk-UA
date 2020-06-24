---
title: Дозволи календаря
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862163"
---
# <a name="calendar-permissions"></a>Дозволи календаря

Користувачі можуть змінити свої власні дозволи календаря з Outlook в Інтернеті або інших клієнтів, але в якості адміністратора, вам може знадобитися для розслідування, а також.  
З Exchange PowerShell командлет покаже вам дозвіл на календар користувача:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Щоб переглянути додаткові відомості див.:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Дозволи календаря використовуються в обміні календарями, щоб переглянути додаткові відомості про спільний доступ до календаря Outlook, перегляньте ці статті:

- [Надання спільного доступу до календаря Outlook іншим користувачам](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Спільний доступ до календаря в Outlook, в Інтернеті для бізнесу](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Для виправлення неполадок календаря можна скористатися засобом [підтримки та відновлення помічника](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .