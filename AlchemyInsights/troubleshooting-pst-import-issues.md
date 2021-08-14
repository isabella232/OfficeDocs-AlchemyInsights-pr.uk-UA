---
title: Виправлення неполадок під час імпорту PST
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1225"
ms.openlocfilehash: 549af832f9c58db1cdd8fbe80b8b5bd2aba9bd937f33116806a9391cbc9a5d4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: uk-UA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972440"
---
# <a name="troubleshooting-pst-import-issues"></a>Виправлення неполадок під час імпорту PST

- Якщо ви імпортуєте дані самого клієнта Outlook див. в статті Вирішення проблем з імпортом [файлу Outlook PST.](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)

- Якщо служба імпорту застрягає, зверніть увагу, що розмір кожного файлу PST, який передається до сховища Azure, не має перевищує 20 ГБ. Файли PST, розмір які перевищує 20 ГБ, можуть вплинути на продуктивність імпорту PST-файлів. Докладні відомості про виправлення неполадок, пов'язаних із завданнями, що застрягли, див. в статі Проблеми, які [впливають на завдання імпорту PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

- Щоб перевірити стан певного завдання імпорту, скористайтеся [get-MailboxImportRequest -batchname.](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest)

- Докладні відомості про службу імпорту див. в огляді [імпорту PST-файлів організації.](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide)
