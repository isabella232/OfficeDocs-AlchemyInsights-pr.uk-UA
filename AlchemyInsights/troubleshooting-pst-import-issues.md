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
# <a name="troubleshooting-pst-import-issues"></a><span data-ttu-id="ccae8-102">Виправлення неполадок під час імпорту PST</span><span class="sxs-lookup"><span data-stu-id="ccae8-102">Troubleshooting PST import issues</span></span>

- <span data-ttu-id="ccae8-103">Якщо ви імпортуєте дані в межах клієнта Outlook, див. статтю [Вирішення проблем з імпортом файлу PST в Outlook](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span><span class="sxs-lookup"><span data-stu-id="ccae8-103">If you are importing within the Outlook client itself, please see [Fix problems importing an Outlook .pst file](https://support.office.com/article/Fix-problems-importing-an-Outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>

- <span data-ttu-id="ccae8-104">Якщо ви використовуєте службу імпорту, і вона припинила відповідати, зверніть увагу, що файл PST, який ви завантажуєте в сховище Azure, не має перевищувати 20 ГБ.</span><span class="sxs-lookup"><span data-stu-id="ccae8-104">If you are using Import Service and it is stuck, please note that each PST file that you upload to the Azure Storage location should be no larger than 20 GB.</span></span> <span data-ttu-id="ccae8-105">Файли завбільшки з понад 20 ГБ можуть сповільнити перебіг імпорту.</span><span class="sxs-lookup"><span data-stu-id="ccae8-105">PST files larger than 20 GB may impact the performance of the PST import process.</span></span>

- <span data-ttu-id="ccae8-106">Щоб перевірити стан певного завдання імпорту, ви можете скористатися командлетом [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span><span class="sxs-lookup"><span data-stu-id="ccae8-106">If you want to verify the status of a specific Import job, you can use [Get-MailboxImportRequest -batchname](https://docs.microsoft.com/powershell/module/exchange/mailboxes/get-mailboximportrequest).</span></span>

- <span data-ttu-id="ccae8-107">Докладні відомості про службу імпорту див. в статті [Імпорт файлів PST у вашій організації](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="ccae8-107">For full details on the import service, please see [Overview of importing your organization's PST files](https://docs.microsoft.com/microsoft-365/compliance/importing-pst-files-to-office-365?view=o365-worldwide).</span></span>
