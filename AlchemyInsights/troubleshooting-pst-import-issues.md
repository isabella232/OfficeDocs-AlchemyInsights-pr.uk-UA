---
title: Виправлення неполадок під час імпорту PST
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 58fdd509fae5e87bf5ae72db5d8926c4367cdd64
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: uk-UA
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991387"
---
# <a name="troubleshooting-pst-import-issues"></a>Виправлення неполадок під час імпорту PST

- Якщо ви імпортуєте дані в межах клієнта Outlook, див. статтю [Вирішення проблем з імпортом файлу PST в Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).

- Якщо ви використовуєте службу імпорту, і вона припинила відповідати, зверніть увагу, що файл PST, який ви завантажуєте в сховище Azure, не має перевищувати 20 ГБ. Файли завбільшки з понад 20 ГБ можуть сповільнити перебіг імпорту.

- Щоб перевірити стан певного завдання імпорту, ви можете скористатися командлетом [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).

- Докладні відомості про службу імпорту див. в статті [Імпорт файлів PST у вашій організації](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).
